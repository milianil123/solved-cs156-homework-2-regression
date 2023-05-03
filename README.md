Download Link: https://assignmentchef.com/product/solved-cs156-homework-2-regression
<br>
The objective of this homework assignment is to predict house prices by deploying various predictive models that accept as inputs, variables that significantly influence the price. We will use 4 different models and compare their performance with respect to their predictive accuracy. Here are the models we will use:

<ol>

 <li>Simple Linear Regression</li>

 <li>Multiple Linear Regression</li>

 <li>Decision Tree Regression</li>

 <li>Random Forest Regression</li>

</ol>




The dataset for this project contains house sale prices. There are 16 column headers:

<ol>

 <li>Waterfront Dummy variable indicating if the house was overlooking a waterfront</li>

 <li>Renovated If the house was renovated</li>

 <li>View An index from 0 to 4 indicating how good the view was. Higher is better</li>

 <li>Condition An index from 1 to 5 on the condition of the apartment. Higher is better</li>

 <li>Grade An index from 1 to 4. Higher the better</li>

 <li>Bedrooms Number of Bedrooms</li>

 <li>Bathrooms Number of Bathrooms (can have 0.5 to indicate half bathroom)</li>

 <li>Sqft_living Square footage of Interior living space</li>

 <li>Sqft_lot Square footage of Interior land space</li>

 <li>Floors Number of floors</li>

 <li>Sqft_above Square footage of the interior living space that is above ground level</li>

 <li>Sqft_basement Square footage of the interior living space that is below ground level</li>

 <li>Yr_built             The year the house was initially built</li>

 <li>Sqft_living15 Square footage of the living area of the nearest 15 neighbors</li>

 <li>Sqft_lot15 Square footage of the land lots of the nearest 15 neighbors</li>

 <li>Price Price of sale</li>

</ol>




<strong><u>Part (A):</u></strong> Data Import, Data Pre-processing

<ol start="3">

 <li>Read the file Housing-Data-one-zip-3.csv</li>

 <li>Convert categorical data: Waterfront, Renovated, View, Condition, Grade</li>

 <li>Transform some data. For example, you may transform the column Yr_built to reflect the age of the building by subtracting Yr_vuilt from 2020.</li>

 <li>Divide the data set into Training set and Test set be</li>

</ol>




We will use the same data set for all 4 prediction algorithms in this assignment. Here are the assumptions for the first 5 fields of the data set and the inputs for your program to do the prediction of house prices. Predict the house price for the following cases (Note: <strong>Age = 2020-Yr_built</strong>)




<table width="359">

 <tbody>

  <tr>

   <td width="79"><strong><u>Assume</u></strong>waterfront</td>

   <td width="76">renovated</td>

   <td width="67">view</td>

   <td width="71">condition</td>

   <td width="67"> grade</td>

  </tr>

  <tr>

   <td width="79"><strong><u> </u></strong></td>

   <td width="76"><u> </u></td>

   <td width="67"><u> </u></td>

   <td width="71"><u> </u></td>

   <td width="67"><u> </u></td>

  </tr>

  <tr>

   <td width="79">0</td>

   <td width="76">0</td>

   <td width="67">0</td>

   <td width="71">3</td>

   <td width="67">3</td>

  </tr>

 </tbody>

</table>




[Bedroom, Bathhrooms, Sqft_living, Sqft_lot, Floors, Sqft_above, Sqft_basement, Age, Sqft_living15, Sqft_lot15]

<ol>

 <li>[3, 0.75, 2510, 20000, 2.0, 2510, 0, 59, 2130, 20000]</li>

 <li>[4, 2.25, 1500, 5393, 2.0, 1500, 0, 21, 1500,    5952]</li>

</ol>

<ul>

 <li>[4, 2.25, 2870, 5393, 2.0, 2870, 0, 21, 1500, 5952]</li>

</ul>

<ol start="3">

 <li>[4, 3.50, 4083, 68377, 2.0, 4083, 0, 15, 2430, 41382]</li>

 <li>[4, 3.50, 4500, 68377, 2.0, 4500, 0, 15, 2430, 41382]</li>

 <li>[4, 3.50, 2870, 68377, 2.0, 2870, 0, 15, 2430, 41382]</li>

</ol>

<ul>

 <li>[4, 3.50, 750, 68377, 2.0,   750, 0, 15, 2430, 41382</li>

</ul>







<strong><u>Part (B):</u></strong>  Use Simple Linear Regression to predict the house price using <strong>Sqft_living</strong> as the independent variable

<ol>

 <li>Print Rsquare</li>

 <li>Plot the linear regression line for the Training Data Set</li>

 <li>Plot the linear regression line for the Test Data Set</li>

 <li>Predict the house prices for the test data set given above.</li>

</ol>

<strong><u>Part (C):</u></strong>  Use Multiple Linear Regression using all variables to predict the house price




<ol>

 <li>Print Rsquare</li>

 <li>Predict the house prices for the test data set given above.</li>

</ol>

<strong><u>Part (D):</u></strong>  Use Decision Tree Regression model to predict the house price

<ol>

 <li>Print Rsquare</li>

 <li>Predict the house prices for the test data set given above.</li>

</ol>

<strong><u>Part (E):</u></strong>  Use Random Forest Regression model (use 10 Random Trees) to predict house price

<ol>

 <li>Print Rsquare</li>

 <li>Predict the house prices for the test data set given above.</li>

</ol>







<strong><u>Summarize your observations:</u></strong>

<ol>

 <li>Tabulate the result as follows:</li>

</ol>







<table>

 <tbody>

  <tr>

   <td width="112">Test Data Point</td>

   <td width="116">Simple Linear Regression</td>

   <td width="116">Multiple Linear Regression</td>

   <td width="116">Decision Tree Regression</td>

   <td width="116">Random Forest Regression</td>

  </tr>

  <tr>

   <td width="112">(i)</td>

   <td width="116">356363.12752274 </td>

   <td width="116">322853.75707537 </td>

   <td width="116">363000 </td>

   <td width="116">405900 </td>

  </tr>

  <tr>

   <td width="112">(ii)</td>

   <td width="116">232887.30257624 </td>

   <td width="116">223043.61780165 </td>

   <td width="116">215000 </td>

   <td width="116">218050 </td>

  </tr>

  <tr>

   <td width="112">(iii)</td>

   <td width="116">400374.31265219 </td>

   <td width="116">402892.93768066 </td>

   <td width="116">299000 </td>

   <td width="116">317590 </td>

  </tr>

  <tr>

   <td width="112">(iv)</td>

   <td width="116">548667.55588001 </td>

   <td width="116">557862.19128196 </td>

   <td width="116">359000 </td>

   <td width="116">474178.8 </td>

  </tr>

  <tr>

   <td width="112">(v)</td>

   <td width="116">599647.17865495 </td>

   <td width="116">588308.23996124 </td>

   <td width="116">359000 </td>

   <td width="116">474178.8 </td>

  </tr>

  <tr>

   <td width="112">(vi)</td>

   <td width="116">400374.31265219 </td>

   <td width="116">469298.50531561 </td>

   <td width="116">359000 </td>

   <td width="116">422128.8 </td>

  </tr>

  <tr>

   <td width="112">(vii)</td>

   <td width="116">141197.33355656 </td>

   <td width="116">314512.83816915 </td>

   <td width="116">194820 </td>

   <td width="116">294180 </td>

  </tr>

  <tr>

   <td width="112">R-Square</td>

   <td width="116">0.6682006794899293 </td>

   <td width="116">0.8072554741507528 </td>

   <td width="116">0.9952504116289396 </td>

   <td width="116">0.9503025303839485 </td>

  </tr>

 </tbody>

</table>




<ol start="2">

 <li>Which predictive model performed the best and why do you think so?

  <ol>

   <li>although the r-squared value for decision tree method is the highest, there are repeated values in the table when the 7<sup>th</sup> parameter is the same, which shows that it isn’t the best estimator. random forest performs somewhat worse than the decision tree in terms of r-squared, but the predictions seem to line up better with the actual data.</li>

  </ol></li>

</ol>




<ol start="3">

 <li>Which variables are most important for prediction? Use Multiple Linear Regression Model to justify your answer. Hint: use <strong>print(regressor.coef_)</strong> to print out the coefficients for the independent variables and focus on the last 10 coefficients.

  <ol>

   <li>we get the following coefficients, where those in boldface and purple are the coefficients of focus:</li>

  </ol></li>

</ol>

8.90689220e+04

4.81272955e+04

1.59078621e+04

7.76704263e+03

3.35765190e+04

<strong>-6.92876340e+03</strong>

<strong>4.32242173e+03</strong>

<strong>4.66709071e+01</strong>

<strong>             6.49099103e-01</strong>

<strong>            -4.18199657e+03</strong>

<strong>             2.63412000e+01</strong>

<strong>             2.03297072e+01</strong>

<strong>            -6.92693042e+02</strong>

<strong>1.71650799e+01</strong>

<strong>2.25297017e+00</strong>

<strong> </strong>

<ol>

 <li>now, we can see the scores of each of the coefficients: we can conclude the most important feature is number of bedrooms, floors, and bathrooms. the others are in boldface below:</li>

</ol>

<ol start="4">

 <li>Feature: 5, Score: -6928.76340</li>

 <li><strong>Feature: 6, Score: 4322.42173</strong></li>

 <li><strong>Feature: 7, Score: 46.67091</strong></li>

 <li><strong>Feature: 8, Score: 0.64910</strong></li>

 <li>Feature: 9, Score: -4181.99657</li>

 <li><strong>Feature: 10, Score: 26.34120</strong></li>

 <li><strong>Feature: 11, Score: 20.32971</strong></li>

 <li>Feature: 12, Score: -692.69304</li>

 <li><strong>Feature: 13, Score: 17.16508</strong></li>

 <li><strong>Feature: 14, Score: 2.25297</strong></li>

</ol>




<strong> </strong>


