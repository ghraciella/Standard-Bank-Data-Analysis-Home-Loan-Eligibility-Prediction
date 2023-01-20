# Standard-Bank-Data-Analysis-Home-Loan-Eligibility-Prediction
Standard Bank Data Analysis for Home Loan Eligibility Prediction



<img src="/imgs/standard.png" width="425"/><img src="/imgs/foragelogo.png" width="425"/>  

<p><h2 align="center"><font color="red">  Project Overview, Task and Solution </font></h2>

<p> Client: Standard Bank Home Loan Department
<p> Client's Industry: Banking and Finance

Standard Bank is one of Africa's biggest lender by assets, the bank aims to improve the current process in which its potential borowers apply for a home loan. The current process involves loan officers manually processing home loan applications which takes 2 to 3 days upon which the applicant will recieve communication or wheter or not they have been granted the loan for the requested amount. 


The main essentials are to understand the business problem and objectives, define the success criteria and project planning:
<li> Business Problem: The process application for a home loan involves loan officers having to manually process them which takes 2 to 3 days, thus applicant’s don’t learn the results of their eligibility on time. </li>

<li> Business Objective: Embrace digital transformation and give the customers a complete set of services such as assessing the creditworthiness of an applicant, checking the status of their loans from the convenience of their mobile devices and much more using machine learning thus speeding up 
the notification process. </li>

<li> Solution: An applicant can apply on any device by filling his/her information (Gender, Marital Status, Income etc.). Upon completion the ML model makes a predict (based on historical data that it has been trained on). The prediction will appear on the device as Accept or Decline on the 
same device in a matter of seconds. </li>

<img src = "/imgs/projectsolution.jpg">




<p><h2 align="center"><font color="red"> Requirements </font></h2>

Follow the data science lifecycle to fulfill the objective. The data science lifecycle (https://www.datascience-pm.com/crisp-dm-2/) includes:

<li> Business Understanding </li>
<li> Data Understanding </li>
<li> Data Preparation </li>
<li> Modelling </li>
<li> Evaluation </li>
<li> Deployment </li>


Working understanding of the CRoss Industry Standard Process for Data Mining (CRISP-DM). CRISP-DM is a process serves as the base for a data science process it has several sequential phases which answers 6 questions:

<img src = "/imgs/CRISP-DM.png">



<li> What does the business need? </li>
<li> What dat do we have/need? is it clean? </li>
<li> How do we organize the data for modelling? </li>
<li> What modelling techniques should we apply? </li>
<li> Which model best meets the business results? </li>
<li> How do stakeholders access the results? </li>





<p><h2 align="center"><font color="red"> Project Process </font></h2>

<li>Overview of Data
        <ul><li>Importing necessary libraries and extraction of datasets using Pandas.</li> 
            <li>The data has 614 unique customer entries and 13 fields containing information with respect to each customer entry, it has both                      numerical and categorical data.</li>
            <li>Our target variable (what we aim to predict) is the Loan Status</li>
        </ul>
    </li>
    
   
<li>Data Preparation
        <ul> 
            <li>Using Python I checked for Missing values and duplicate data. </li>
            <li>Exploratory Data Analysis(EDA) on historical data (train data) and test data.</li>       
        </ul>
    </li>
 

<li>Modelling
        <ul><li> AutoSklearn AutoML. </li>
        <li> Bespoke ML: Logistic Regression Model. </li>        
        </ul>
        </li>   
 
 
 <li>Model Evaluation
        <ul><li> Evaluation Metric used is Accuracy</li>     
        </ul>
 </li>    


</p>


<p><h2 align="center"><font color="red"> Answers to Questions posed by The Home Loans Department Manager based of EDA </font></h2>

1. Overview of the data.
   - The train data contains 614 Rows and total 13 columns with 4 float columns, 1 integer column and 8 object columns.

   - The test data contains 367 Rows and total 12 columns with 3 float columns, 2 Integer columns and 7 object columns.

2. What data quality issues exist in both train and test?
   - Both datasets have some missing values;

   - For the train dataset there was 149 missing/NULL data where: 1: Gender has 13, Married has 3, Dependents has 15, Self_Employed has 32, LoanAmount has 22, Loan_Amount_Term has 14 and Credit_History has 50 missing values respectively.
 
   - For the test dataset there was 84 missing/NULL data where: 1: Gender has 11, Dependents has 10, Self_Employed has 23, LoanAmount has 5, Loan_Amount_Term has 6 and Credit_History has 29 missing values respectively.

   - There were no duplicate values in both train and test datasets.

3. How do the loan statuses compare? i.e. what is the distrubition of each?
   - For the Distribution of loan status: Yes(Y) or No(N), there were 422 loans with a Yes status and 192 loans with No status. 
   
4. How do women and men compare when it comes to defaulting on loans in the historical dataset?
   - Based of the historical dataset, it shows that men have a higher loan status of Yes(and No) than women do.
   
5. How many of the loan applicants have dependents based on the historical dataset?
   - From the historical dataset, it shows there were 269 loan applicants who have dependents.
   
6. How does the income of those who are employed compare to those who are self-employed based on the historical dataset?
   - Based of the descriptive statistics carried out on the historical dataset, it show that:
     - On an average the income of the self-employed is 7380 compared to the income of those employed which is 5049.
     
     - The number of self-employed is 82 which is low compared to the employed which is 500.
     
7. Are applicants with a credit history more likely to default than those who do not have one?
   - Yes, applicants with credit histories are more likely to default than those who don't have them.
   
8. Is there a correlation between the applicant's income and the loan amount they applied for?
   - Yes.


<p><h2 align="center"><font color="red"> Analysis and Visualization </font></h2>

For my data isualization to provide insights, I used python libraries, such matplotlib and seaborn. 

### Distribution Data of Loan Status

Analysis: The Loan Status gives an indication of customers who applied for a loan versus who didn‘t. It indicates 422 persons have an active loan
application while 192 don‘t. 

<li> Yes(Y) and No(N) </li>

<img src = "/imgs/comparisonloanstatus.jpg">


### Comparison of Loan Status based on Gender

Analysis: There are 489 Males and 112 Females. The Comparison shows that based on the historical dataset, it shows that men have a higher loan status than women do.


<li> Yes(Y) and No(N) </li>
<li> Male(M) and Female(F) </li>


<img src = "/imgs/comparisonloanstatusgender.jpg">


### Comparison of Loan Status based on Gender

Analysis: There are 475 customers with credit histories and 112 without. The comparison shows that based on the historical dataset, that applicants with credit histories are more likely to default than those who don't have them.

<li> Yes(Y) and No(N) </li>
<li> No Credit History (0) and Credit History(1) </li>


<img src = "/imgs/comparisoncredithistoryloanstatus.jpg">


### Confusion Matrix

Analysis: The confusion matrix shows there is a correlation between Applicant‘s Income and the loan amount requested.



<img src = "/imgs/confusionmatrix.jpg">




<p><h2 align="center"><font color="red"> Recommendations </font></h2>
 

<ul>
<li> The evaluation shows that the AutoML performs better than the Bespoke ML.</li>
<li> We get quicker results AutoML which helps us save on time and resources.</li>
<li> AutoML gives us less insight on our data and less customizable compared to Bespoke ML.</li>
<li> Using the Bespoke ML helps us fully understand all the details of our data, details of the 
algorithm and how it can be further customized also improved to meet the business needs 
for the company.</li>




