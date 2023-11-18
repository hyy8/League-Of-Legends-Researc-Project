# League-Of-Legends-Research-Project
<!DOCTYPE html>
<html>
<body>
<h1>Hello World</h1>
<p>I'm hosted with GitHub Pages.</p>
<p>
<strong> Here is the head of our side DataFrame: </strong>   
</p>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: right">side</th>
      <th style="text-align: right">result</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Blue</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Red</td>
      <td>0</td>
    </tr>
    <tr>
      <td>Blue</td>
      <td>0</td>
    </tr>
    <tr>
      <td>Red</td>
      <td>1</td>
    </tr>
    <tr>
      <td>Blue</td>
      <td>1</td>
    </tr>
  </tbody>
</table>
</div>
<p>
<strong> Below is the table of result distribution: </strong>   
</p>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: right">result_side</th>
      <th style="text-align: right">Loss</th>
      <th style="text-align: right">Win</th>
      <th style="text-align: right">Loss_prop</th>
      <th style="text-align: right">Win_prop</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>Blue</th>
      <td>5026</td>
      <td>5772</td>
      <td>10798</td>
      <td>0.465457</td>
      <td>0.534543</td>
    </tr>
    <tr>
      <th>Red</th>
      <td>5772</td>
      <td>5026</td>
      <td>10798</td>
      <td>0.534543</td>
      <td>0.465457</td>
    </tr>
  </tbody>
</table>
</div>
<h2>Univariate Analysis: </h2>
<p> </p>
<h2>Assessment of Missingness: </h2>
<h3>Missingness Dependency: </h3>
<p> Below is the observed distribution when "firstdragon" was not missing:</p>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: right">barons</th>
      <th style="text-align: right"> No Missing First Dragon</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0.0</th>
      <td>0.438794</td>
    </tr>
    <tr>
      <th>1.0</th>
      <td>0.396283</td>
    </tr>
    <tr>
      <th>2.0</th>
      <td>0.148245</td>
    </tr>
    <tr>
      <th>3.0</th>
      <td>0.015261</td>
    </tr>
    <tr>
      <th>4.0</th>
      <td>0.001417</td>
    </tr>
  </tbody>
</table>
</div>
<p> Below is the observed distribution when "firstdragon" was missing:</p>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: right">barons</th>
      <th style="text-align: right">Missing First Dragon</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0.0</th>
      <td>0.859982</td>
    </tr>
    <tr>
      <th>1.0</th>
      <td>0.113656</td>
    </tr>
    <tr>
      <th>2.0</th>
      <td>0.024519</td>
    </tr>
    <tr>
      <th>3.0</th>
      <td>0.001779</td>
    </tr>
    <tr>
      <th>4.0</th>
      <td>0.000063</td>
    </tr>
  </tbody>
</table>
</div>

<p> The Missingness of "firstdragon" does not depends on "dragons"</p>
<p> Below is the observed distribution when "firstdragon" was not missing:</p>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: right">dragons</th>
      <th style="text-align: right"> No Missing First Dragon</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>3.0</th>
      <td>0.229671</td>
    </tr>
    <tr>
      <th>2.0</th>
      <td>0.224166</td>
    </tr>
    <tr>
      <th>1.0</th>
      <td>0.190702</td>
    </tr>
    <tr>
      <th>4.0</th>
      <td>0.174951</td>
    </tr>
    <tr>
      <th>0.0</th>
      <td>0.151679</td>
    </tr>
    <tr>
      <th>5.0</th>
      <td>0.027523</td>
    </tr>
    <tr>
      <th>6.0</th>
      <td>0.001308</td>
    </tr>
  </tbody>
</table>
</div>

<p> Below is the observed distribution when "firstdragon" was missing:</p>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: right">dragons</th>
      <th style="text-align: right">Missing First Dragon</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>3.0</th>
      <td>0.304841</td>
    </tr>
    <tr>
      <th>4.0</th>
      <td>0.281182</td>
    </tr>
    <tr>
      <th>2.0</th>
      <td>0.227867</td>
    </tr>
    <tr>
      <th>1.0</th>
      <td>0.136284</td>
    </tr>
    <tr>
      <th>5.0</th>
      <td>0.047645</td>
    </tr>
    <tr>
      <th>6.0</th>
      <td>0.002181</td>
    </tr>
  </tbody>
</table>
</div>




  
</body>
</html>
