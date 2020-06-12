# SAS
This repository contains SAS related Projects / Models / Codes etc .

# 


Modular Code File -

Run transformation code befor analysis code
Steps -

Read in Data
Keep Only Native Variables Needed
Apply Exclusions
Add transformed variable from Data Dictionary
....
Analysis Code 

Part 1 : Descriptive Analysis

Code with prefix 
100s - trnsformation Code 
200s - Plot Code
300s - Descriptive analysis
400s - Extras

part 2 - 

Regression Analysis 

500 - Linear
600 - Logistic 
700- extra

---

Dataset naming - 
BRFSS_ - Native dataset 
Copy of BRFSS_a to BRFSS_b ( Remove unnecessary Columns)
copy BRFSS_b top BRFSS_c and remove exclusions

Hypothesis - 

A hypothesis which will be best for descriptive analysis and regression . 

Component of Hypotesis - 
Subpopulation ( Sample Populaton )
 
We need two hypothesis as output from Linear regression is continuous and that from logistic regression is binary

===============================================
Subpopulation - Veterans
Exposure - Having Diabetes 
Disease - Linear regression ( Avg sleep per night)
          logistic regression ( Having Asthma)
		  
Hypothesis - 
1. Among veterans diabetes status is statistically significantly associated with average hours of sleep per night

2. Among veterans diabetes status is statistically significantly associated asthama status

.xpt format similar to zip format of .sas7bdat , we need to unpack .xpt to .sas7bdat file 

We also need special lib name for for .xpt 

Typical libname :

Libname p "c:\sas";
run;

for reading *.xpt file 

Libname p "c:\sas";
run;

libname XPTfile xport "c:\sas\name.xpt";
run;





