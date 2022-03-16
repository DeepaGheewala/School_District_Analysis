# School District Analysis


# Overview
## Background

Maria was informed by the school board that they suspect the math and reading scoring of 9th grade from Thomas High School might not be be correct. Due to that they request to perform analysis of school data without Thomas High School 9th grade math and reading scores.

## Purpose
Maria was provided with student funding and student scoring data in two csv files (School Data School_data.csv and Student Data student_data.csv). City school Board asked to analyse these data files and provide different results which will help the School Authorities to make decision in school budgetting and school performaces across district. 

The Analysis Report will have 
* [The District Summary] (#The-District-Summary)
* [The School Summary] (#The-School-Summary)
* [Thomas High School Performance Impact](#Thomas-High-School-Performance-Impact)
* [Top and Bottom 5 Performing Schools] (#Top-&-Bottom-5-Performing-Schools)
* [Average Math and Reading Score For Each Grade](#Average-Math-and-Reading-Score-For-Each-Grade
* [Scores by School Spending Per Student](#Scores-by-School-Spending-Per-Student)
* [Scores by School Size](#Scores-by-School-Size)
* [Scores by School Type](#Scores-by-School-Type)

# Results 

  
## Thomas High School data updated with Nan

## The District Summary
Below we can see District Summary data comparison with 9th grade and without 9th grade.

*With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/88678f4df58877752fee43029444b0dfae800248/Resources/district_summary_withoutNAN.png" />

*9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/88678f4df58877752fee43029444b0dfae800248/Resources/district_summary_withNAN.png" />

The above comparison shows that 
* Average Math Score, % Passing Math, % Passing Reading and %Overall Passing has little higher values.
* Average Reading Score is same in both the cases.
* Overall the impact to district summary is minimal
* If we assume the data of 9th grade was honest then it shows 9th Grader have performed well so the average score has increased

As the data of 9th grade was updated to Nan, it was not included for calculations


## The School Summary
### ***School summary comparison based on describe()***

*With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/e4c96b740409981d8bad2ffa80d06cf5ee36f19d/Resources/school%20summary%20describe%20without%20nan.png" />

*9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/e4c96b740409981d8bad2ffa80d06cf5ee36f19d/Resources/school%20summary%20describe%20with%20nan.png" />

### ***School summary comparison based on data table***

*With 9th Grade data* [All Data](https://github.com/DeepaGheewala/School_District_Analysis/blob/861454c90ce7be18e3c6d97767c30d84337a2c88/Resources/school%20summary%20with%20nan.png)
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/27ac2baa347eb8d3497214182c2aa3e95fd7f764/Resources/school%20summary%20with%20nan%20THS.png" />

*9th Grade data updated to Nan* [ALL Data](https://github.com/DeepaGheewala/School_District_Analysis/blob/861454c90ce7be18e3c6d97767c30d84337a2c88/Resources/school%20summary%20without%20nan.png)
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/27ac2baa347eb8d3497214182c2aa3e95fd7f764/Resources/school%20summary%20without%20nan%20THS.png" />

## Thomas High School Performance Impact

Thomas School Performance improves slightly when 9th grade data is considered.
*With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/27ac2baa347eb8d3497214182c2aa3e95fd7f764/Resources/school%20summary%20with%20nan%20THS.png" />

*9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/27ac2baa347eb8d3497214182c2aa3e95fd7f764/Resources/school%20summary%20without%20nan%20THS.png" />

## Top and Bottom 5 Performing Schools
### ***Top Ranking*** 
 Thomas High School ranks second among the list of all schools with or without 9th grader data. This shows that Thomas school has been performing well and 9th grader data might be honest to the standards of the school.
 
 *With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/e4c96b740409981d8bad2ffa80d06cf5ee36f19d/Resources/Top%20performing%20schools%20with%20Nan.png" />

*9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/e4c96b740409981d8bad2ffa80d06cf5ee36f19d/Resources/Top%20performing%20schools%20without%20Nan.png" />

### ***Bottom Ranking***
As Thomas High School is not included in the bottom school list there is no impact to the bottom performing schools.

*With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/8ab2550d5bff92aa099e9fe928c1014d4389450c/Resources/Bottom%20performing%20schools%20with%20Nan.png" />

*9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/8ab2550d5bff92aa099e9fe928c1014d4389450c/Resources/Bottom%20performing%20schools%20without%20Nan.png" />

## Average Math and Reading Score For Each Grade
### ***Math Score Grading***
Thomas School's 9th Grade Math score data average is nearly similar with other grade average scores

<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/8ab2550d5bff92aa099e9fe928c1014d4389450c/Resources/grade%20wise%20math%20average%20THS.png" />

### ***Reading Score Grading***
Thomas School's 9th Grade Reading score data average is nearly similar with other grade average scores

<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/8ab2550d5bff92aa099e9fe928c1014d4389450c/Resources/grade%20wise%20reading%20average%20THS.png" />

## Scores by School Spending Per Student

## Scores by School Size

## Scores by School Type

#Summary
