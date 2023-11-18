# League-Of-Legends-Research-Project
<!DOCTYPE html>
<html>
<body>
<h2>Introduction:</h2>
<p> </p>

<h2> Cleaning and EDA (Exploratory Data Analysis):</h2>
<h3> Data Cleaning</h3>
<p>
<strong> Here is the head of our side DataFrame: </strong>   
</p>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: left">side</th>
      <th style="text-align: left">result</th>
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
<p>
<strong> Below is the table of result distribution: </strong>   
</p>
<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: left">result_side</th>
      <th style="text-align: left">Loss</th>
      <th style="text-align: left">Win</th>
      <th style="text-align: left">Total</th>
      <th style="text-align: left">Loss_prop</th>
      <th style="text-align: left">Win_prop</th>
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
<h3>Univariate Analysis: </h3>
<iframe src="assets/pie.html" width=800 height=600 frameBorder=0></iframe>
<h3>Bivariate Analysis:</h3>
<iframe src="assets/Bivariate3.html" width=800 height=600 frameBorder=0></iframe>

  
<p> </p>
<h2>Assessment of Missingness: </h2>
<h3>NMAR Analysis: </h3>
<h3>Missingness Dependency: </h3>
<p> Below is the observed distribution when "firstdragon" was not missing:</p>

<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: left">barons</th>
      <th style="text-align: left"> No Missing First Dragon</th>
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

<p> Below is the observed distribution when "firstdragon" was missing:</p>

<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: left">barons</th>
      <th style="text-align: left">Missing First Dragon</th>
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

<p> observed_tvd: 0.42118789454515004 </p>
<p> p_value: 0.0 </p>
<iframe src="assets/barons.html" width=800 height=600 frameBorder=0></iframe>

<p> The Missingness of "firstdragon" does not depends on "dragons"</p>
<p> Below is the observed distribution when "firstdragon" was not missing:</p>

<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: left">dragons</th>
      <th style="text-align: left"> No Missing First Dragon</th>
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


<p> Below is the observed distribution when "firstdragon" was missing:</p>

<table border="1" class="dataframe">
  <thead>
    <tr>
      <th style="text-align: left">dragons</th>
      <th style="text-align: left">Missing First Dragon</th>
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

<p> observed_tvd: 0.021956259443855583</p>
<p> p_value: 0.8</p>
<iframe src="assets/dragons.html" width=800 height=600 frameBorder=0></iframe>
<h2> Hypothesis Testing: </h2>
<p>
  <strong>Null Hypothesis (H0):</strong>
  The win rate of red side is equal to the win rate of the blue side.
</p>
<p>
  <strong>Alternative Hypothesis (H1):</strong>
  The win rate of red side is different from the win rate of the blue side.
</p>
<p>
  <strong>t_statistic:</strong>
  "We are using the difference between the two sample means divided by 
  the standard error of the difference between those means to calculate the t_statistic."
</p>
<p>
  <strong>Significant Level: 0.05</strong>
</p>
<p>
  <strong>p_value:2.86252172582626e-24</strong>
</p>
<p>
  <strong>Conclusion:Reject the null hypothesis.</strong>
</p>




  
</body>
</html>
