# SAS
This repository contains SAS related Projects / Models / Codes etc .

# 


#Modular Code File -

Run transformation code befor analysis code
Steps -

1. Read in Data
2. Keep Only Native Variables Needed
3. Apply Exclusions
4. Add transformed variable from Data Dictionary
5. ....
& last step would be Analysis Code 

#Part 1 : Descriptive Analysis

Code with prefix 
100s - trnsformation Code 
200s - Plot Code
300s - Descriptive analysis
400s - Extras

#part 2 - 

Regression Analysis 

500 - Linear
600 - Logistic 
700- extra

---

#Dataset namingconvension - 
BRFSS_ - Native dataset 
Copy of BRFSS_a to BRFSS_b ( Remove unnecessary Columns)
copy BRFSS_b top BRFSS_c and remove exclusions

#Hypothesis Declaration - 
As we are using two regeression for analysis - Linear and logistic so we must schoose a hypothesis which will be best for descriptive analysis and regression . 

#Component of Hypotesis - 
Subpopulation ( Sample Populaton )
 
We need two hypothesis as output from Linear regression is continuous and that from logistic regression is binary

=========================================
Subpopulation - Veterans
Exposure - Having Diabetes 
Disease - Linear regression ( Avg sleep per night)
          logistic regression ( Having Asthma)
		  
# Hypothesis - 
1. Among veterans diabetes status is statistically significantly associated with average hours of sleep per night

2. Among veterans diabetes status is statistically significantly associated asthama status

# Sas Big Data
In SAS the general sas file format is *.sasbdat but this file is bigger (in size) in nature compare to the .csv from which it as generated or the .csv having the same data. *
For saving too huge data SAS came with up a new format called .xpt. 

.xpt format similar to zip format of .sas7bdat , we need to unpack .xpt to .sas7bdat file 

We also need special lib name for for .xpt 
#Some code are below for reference 

Typical libname :

Libname p "c:\sas";
run;

for reading *.xpt file 

Libname p "c:\sas";
run;

libname XPTfile xport "c:\sas\name.xpt";
run;





