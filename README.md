# SCHOOL DISTRICT ANALYSIS
_Analyzing student grades and school budget to reveal trends_


## Overview of the Project
A school board has identified academic dishonesty in the 9th grade results presented by one of its schools. 
The purpose of this project was to rid the previous dataset off this discrepancy by replacing with NaN all the grades in question and analyze the data again to show if the information presented from an earlier analysis will be affected by this change.

## Results

* **District Summary**

To obtain the clean district summary of school grades and budget required that all the 9th grades scores of Thomas High be replaced with NaN. This involved the use of the "loc" property to select all the reading and maths scores from the 9th grade and with the help of "numpy" replaced them with NaN.
In order to get the right metrics, a new student count was then generated by subtracting the total number of 9th grade-students of Thomas High School from the entire student population of the school district.
Though some level of change was witnessed from the analysis (eg. Average math score for the district changed from 78.99 to 78.93), the information generated after the changes showed no significant departure from the results of the earlier analysis. The district summary data remained same.


_*District summary before replacing math and reading sores*_

![Alt text](https://github.com/emmanuelbrim/School_District_Analysis/blob/main/Resources/Dsummaryoriginal.PNG)

_*District summary after replacing math and reading scores*_

![Alt text](https://github.com/emmanuelbrim/School_District_Analysis/blob/main/Resources/Dsummaryfinal.PNG)


* **School Summary**

To generate a clean School summary invoved selecting all the students of Thomas High School, except 9th grades students and finding the pecentages of their reading and maths scores using the new student total. The school summary dataframe was then updated with the results using the 'loc' method to reflect the changes in the percentage of students from Thomas High School who passed_math, reading and in both subjects. 
Once again though there was a change in the percentages from Thomas High School, the school summary data showed no change. 
The data showed that charter schools still dominated the top list of schools in the district and the bottom 5 schools were still of the district type. 

_Bottom 5 schools before cleaning data_

![Alt text](https://github.com/emmanuelbrim/School_District_Analysis/blob/main/Resources/bottomschooloriginal.PNG)

_Bottom 5 schools after cleaning data_

![Alt text](https://github.com/emmanuelbrim/School_District_Analysis/blob/main/Resources/bottomschoolfinal.PNG)



* **Thomas High School Performance**

A change in performacnce was expected since 9th grade reading and maths scores were replaced with higher percentages. However the change in scores didnot contribute to a change in the performance of Thomas High School. The data showed that the school maintained its position as the second best school in the district after Cabrera High School. 

_Thomas High Performance before change

![Alt text](https://github.com/emmanuelbrim/School_District_Analysis/blob/main/Resources/topschoolsoriginal.PNG)


_Thomas High Performance after change_

![Alt text](https://github.com/emmanuelbrim/School_District_Analysis/blob/main/Resources/topschoolfinal.PNG)



* * **Scores by grade**
The scores by grade remained same though 9th grade scores from Thomas high was replaced with NaN. 
* * **Scores by school spending**
The school spending data showed no change
* * **Scores by school size**
The school size was not affected by the changes in the data from Thomas High School
* * **Scores by school type**
Like all others the type summary remained same after the analysis.



* **Summary**
In conclusion, the analysis after the reading and math scores were replaced did indicate a change in the initail statistics but this led to no signifiacnt change in the final information generated. School and distrcit summaries showed same results for all points as well as the performance of Thomas High school.  


