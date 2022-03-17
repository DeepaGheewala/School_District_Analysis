# School District Analysis


# Overview
## Background

Maria was informed by the school board that they suspect the math and reading scoring of 9th grade from Thomas High School might not be be correct. Due to that they request to perform analysis of school data without Thomas High School 9th grade math and reading scores.

## Purpose
Maria was provided with student funding and student scoring data in two csv files ([School Data.csv](https://github.com/DeepaGheewala/School_District_Analysis/blob/ed29fbd8bd5eec737fb818b798a48d03aa038e1b/Resources/schools_complete.csv) and [Student Data.csv](https://github.com/DeepaGheewala/School_District_Analysis/blob/ed29fbd8bd5eec737fb818b798a48d03aa038e1b/Resources/students_complete.csv)). City school Board asked to analyse these data files and provide different results which will help the School Authorities to make decision in school budgetting and school performaces across district. 

The Analysis Report need to have 
* [The District Summary](#The-District-Summary)
* [The School Summary](#The-School-Summary)
* [Thomas High School Performance Impact](#Thomas-High-School-Performance-Impact)
* [Top And Bottom 5 Performing Schools](#Top-And-Bottom-5-Performing-Schools)
* [Average Math And Reading Score For Each Grade](#Average-Math-And-Reading-Score-For-Each-Grade)
* [Scores by School Spending Per Student](#Scores-by-School-Spending-Per-Student)
* [Scores by School Size](#Scores-by-School-Size)
* [Scores by School Type](#Scores-by-School-Type)

# Results 
After processing Student data and School data, the following data outcomes were listed.
  
## Thomas High School data updated with Nan
In order to update the data of 9th grader Thomas High School the following code was written
```{python}
#  Step 3. Refactor the code in Step 2 to replace the math scores with NaN.

student_data_df.loc[(student_data_df["grade"] == "9th") & 
                    (student_data_df["school_name"] == "Thomas High School"), "math_score"] = np.nan
student_data_df

```
## The District Summary
Below we can see District Summary data comparison with 9th grade and without 9th grade.

- *With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/88678f4df58877752fee43029444b0dfae800248/Resources/district_summary_withoutNAN.png" />

- *9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/88678f4df58877752fee43029444b0dfae800248/Resources/district_summary_withNAN.png" />

The above comparison shows that 
* Average Math Score, % Passing Math, % Passing Reading and %Overall Passing has little higher values with 9th grader Thomas High School data.
* Average Reading Score is same in both the cases.
* Overall the impact to district summary is minimal
* If we assume the data of 9th grade was honest then it shows 9th Grader have performed well so the average score has increased
* Even as there is not much difference in averages, 9th grader data might be honest.


## The School Summary
### ***School summary comparison based on describe()***
 The below image comparison gives are very major difference in the **50th percentile** data.  
 There are other few considerable differences noticed in mean, std, min, 25th percentile.  
 Also remaining data has minute differences.
 
- *With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/e4c96b740409981d8bad2ffa80d06cf5ee36f19d/Resources/school%20summary%20describe%20without%20nan.png" />

- *9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/e4c96b740409981d8bad2ffa80d06cf5ee36f19d/Resources/school%20summary%20describe%20with%20nan.png" /> 

### ***School summary comparison based on data table***
Overall there is negligible difference in the data

- *With 9th Grade data* [All Data](https://github.com/DeepaGheewala/School_District_Analysis/blob/861454c90ce7be18e3c6d97767c30d84337a2c88/Resources/school%20summary%20with%20nan.png)
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/27ac2baa347eb8d3497214182c2aa3e95fd7f764/Resources/school%20summary%20with%20nan%20THS.png" />

- *9th Grade data updated to Nan* [ALL Data](https://github.com/DeepaGheewala/School_District_Analysis/blob/861454c90ce7be18e3c6d97767c30d84337a2c88/Resources/school%20summary%20without%20nan.png)
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/27ac2baa347eb8d3497214182c2aa3e95fd7f764/Resources/school%20summary%20without%20nan%20THS.png" />

## Thomas High School Performance Impact

Thomas School Performance improves slightly when 9th grade data is considered.

- *With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/27ac2baa347eb8d3497214182c2aa3e95fd7f764/Resources/school%20summary%20with%20nan%20THS.png" />

- *9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/27ac2baa347eb8d3497214182c2aa3e95fd7f764/Resources/school%20summary%20without%20nan%20THS.png" />

## Top And Bottom 5 Performing Schools
### ***Top Ranking*** 
 Thomas High School ranks second among the list of all schools with or without 9th grader data. This shows that Thomas school has been performing well and 9th grader data might be honest to the standards of the school.
 
- *With 9th Grade data*  
 
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/e4c96b740409981d8bad2ffa80d06cf5ee36f19d/Resources/Top%20performing%20schools%20with%20Nan.png" />

- *9th Grade data updated to Nan*  

<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/e4c96b740409981d8bad2ffa80d06cf5ee36f19d/Resources/Top%20performing%20schools%20without%20Nan.png" />

### ***Bottom Ranking***
As Thomas High School is not included in the bottom school list there is no impact to the bottom performing schools.

- *With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/8ab2550d5bff92aa099e9fe928c1014d4389450c/Resources/Bottom%20performing%20schools%20with%20Nan.png" height="250" width="1000"/>

- *9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/8ab2550d5bff92aa099e9fe928c1014d4389450c/Resources/Bottom%20performing%20schools%20without%20Nan.png" height="250" width="1000"/>

## Average Math And Reading Score For Each Grade
### ***Math Score Grading***
Thomas School's 9th Grade Math score data average is nearly similar with other grade average scores

<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/8ab2550d5bff92aa099e9fe928c1014d4389450c/Resources/grade%20wise%20math%20average%20THS.png"  height="250" width="1000" />

### ***Reading Score Grading***
Thomas School's 9th Grade Reading score data average is nearly similar with other grade average scores

<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/8ab2550d5bff92aa099e9fe928c1014d4389450c/Resources/grade%20wise%20reading%20average%20THS.png"  height="250" width="1000"/>

## Scores by School Spending Per Student
The spending bin $630-644 only has difference in data, this is because it has Thomas High School data falling in this bin.

- *With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/20377d541a650b833b62fe8e0b83157269aa856c/Resources/spending%20bins%20without%20Nan.png" />

- *9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/20377d541a650b833b62fe8e0b83157269aa856c/Resources/spending%20bins%20with%20Nan.png" />


## Scores by School Size
As Thomas High School falls into the catagory of Medium sized school, the data of medium sized bin has variations. Rest of the two bins are not impacted.

- *With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/20377d541a650b833b62fe8e0b83157269aa856c/Resources/Performance%20based%20on%20School%20Size%20without%20NaN.png" />

- *9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/ed29fbd8bd5eec737fb818b798a48d03aa038e1b/Resources/Performance%20based%20on%20School%20Size%20with%20NaN.png" />

## Scores by School Type
Thomas High School is a charter school, therefore we notice minor differences in the data.

- *With 9th Grade data*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/20377d541a650b833b62fe8e0b83157269aa856c/Resources/Performance%20based%20on%20School%20Type%20without%20NaN.png" />

- *9th Grade data updated to Nan*
<img src="https://github.com/DeepaGheewala/School_District_Analysis/blob/20377d541a650b833b62fe8e0b83157269aa856c/Resources/Performance%20based%20on%20School%20Type%20with%20NaN.png" />

# Summary of the School District Analysis
From the above analysis we can conclude the following:
- Thomas High School ranked second irrespective of including 9th grade data or not.
- 9th grade maths and reading score average is nearly similar to the other grade averages.
- Impact on mean, standard deviation, min, 25th percentile was noticable. 
- Impact on 50th percentile has been considerably high, which shows most 9th grader data fall into 50th percentile. 
- Due to overall less impact on all data and nearly similar averages of 9th grader compared to other graders, it looks like the 9th grader data could be honest
- District data and overall grading data shows better performance including 9th grader data.


# Resources
Applications
1) Jupyter Notebook
2) Python

Dependent Libraries
1) Pandas
2) Numpy
