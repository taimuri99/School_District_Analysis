# School District Analysis
Analysis done using Python on Jupyter Notebook using and manipulating Panda Dataframes.
## Overview of the school district analysis.
The purpose of the original analysis was to analyze the school and students data to see the performance of students and schools in reading and maths on a district level. Performance was also calculated for each grade level, for groups of school size and types and also by spending budget per student. The challenge tasked us to review the data due to academic dishonesty for 9th Grade students in Thomas High School for both reading and maths. To  uphold state-testing standards, the said results were changed to NaNs while the rest of the data remained intact. After replacing the data, the school district analysis was performed again.
## Results
After editing the code to remove grades by assigning them NaNs and analysing the district school data again, the following results were found.
### How is the district summary affected?
Below is the original district summary before the grades removal:

<img width="923" alt="OriginalDistrictSummary" src="https://user-images.githubusercontent.com/87828174/134785070-5ce3b060-2af1-4ac5-a893-6b3c9887bd79.png">

And here is the updated district summary:

<img width="921" alt="NewDistrictSummary" src="https://user-images.githubusercontent.com/87828174/134785075-8f604272-0463-47d0-be64-f1421f4d7a5a.png">

As you can see average math scores decreased after removing the affected student grades. The average reading scores were not affected and remained the same. The maths, reading and overall passing percentage also decreased.
### How is the school summary affected?
Below is the original school summary:

<img width="954" alt="Columns heads" src="https://user-images.githubusercontent.com/87828174/134786756-d28a2aff-9367-4151-8cfa-0be577bc3d36.png">
<img width="954" alt="OriginalSchoolSummaryTHS" src="https://user-images.githubusercontent.com/87828174/134785984-27718242-80f7-4a1a-9d88-a463c148f95f.png">

Here is the school summary dataframe with NaN values of 9th grade included. The values are innaccurate as they count Thomas High School 9th grade results as NaNs which affects the overall performance of the school therefore decreasing the performance values by large amounts:

<img width="957" alt="Columns heads" src="https://user-images.githubusercontent.com/87828174/134786756-d28a2aff-9367-4151-8cfa-0be577bc3d36.png">
<img width="957" alt="SchoolSummaryCounting9th" src="https://user-images.githubusercontent.com/87828174/134785986-0320d335-9585-4069-8ee7-155ae8878ed4.png">

And here is the updated district summary after taking the math, reading and overall scores and passing percentages for grades 10, 11 and 12 and replacing the innacurate values in the previous dataframe with them. This was done to mantain academic integrity by not counting the 9th grade results at all and only counting and creating a summary with 10th, 11th and 12th grade results for Thomas High School.

<img width="961" alt="Columns heads" src="https://user-images.githubusercontent.com/87828174/134786756-d28a2aff-9367-4151-8cfa-0be577bc3d36.png">
<img width="961" alt="NewSchoolummary" src="https://user-images.githubusercontent.com/87828174/134785991-e3efc82b-4076-4b18-b23d-8f15b16f137b.png">

Only the results of Thomas High School are included as the rest of the schools had the same results and analysis in all dataframes. As you can see the performance results show that the difference between the original and removed 9th grade results dataframe do not differ by that much. Although the original scores and passing percentages are slightly higher, academic integrity has been maintained to an extent as the school summaries match to 2 decimal places. 

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
Here are the top performing schools before the grades were removed from Thomas High School 9th grade:

<img width="993" alt="OriginalTopSchools" src="https://user-images.githubusercontent.com/87828174/134786494-f94fd459-f5c4-493e-a7a3-5978350449d2.png">

And here are the top performing schools after the grades are removed and only 10th, 11th and 12th grade results are considered for Thomas High School:

<img width="990" alt="NewTopSchools" src="https://user-images.githubusercontent.com/87828174/134786513-1083c6a5-72a8-4080-807f-04ae3ffba06a.png">

As you can see the top 5 schools remain the same with Thomas High School still performing well at second place. Although the passing percentages and reading and maths scores have decreased, the overall performance with respect to other schools remains the same thus sustaining the integrity of the school and district analysis. The bottom 5 schools are unchanged as well.

### How does replacing the ninth-grade scores affect the following?
#### Math and reading scores by grade
Here are the original math performances per grade for Thomas High School:

<img width="425" alt="Columns" src="https://user-images.githubusercontent.com/87828174/134786813-bff2111a-324e-4a5d-99d0-bca789d4d6c0.png">
<img width="424" alt="OriginalTHSMaths" src="https://user-images.githubusercontent.com/87828174/134786808-78b92957-3d9c-4863-9847-f2df8c5f5a7a.png">

and here are the updated perfomances:

<img width="425" alt="Columns" src="https://user-images.githubusercontent.com/87828174/134786813-bff2111a-324e-4a5d-99d0-bca789d4d6c0.png">
<img width="424" alt="NewTHSMaths" src="https://user-images.githubusercontent.com/87828174/134786862-237865ee-865a-442b-bcb5-0662345d7e4b.png">

Similarly the original reading performances per grade for Thomas High School:

<img width="425" alt="Columns" src="https://user-images.githubusercontent.com/87828174/134786813-bff2111a-324e-4a5d-99d0-bca789d4d6c0.png">
<img width="424" alt="OriginalReadTHS" src="https://user-images.githubusercontent.com/87828174/134786961-a1eb6976-4da5-4ccc-87a0-6088298e05ec.png">

and the updated performances:

<img width="425" alt="Columns" src="https://user-images.githubusercontent.com/87828174/134786813-bff2111a-324e-4a5d-99d0-bca789d4d6c0.png">
<img width="426" alt="NewReadTHS" src="https://user-images.githubusercontent.com/87828174/134786970-d6900419-9247-4046-a06d-637a98d33c7f.png">

The only information we get from these dataframe screenshots is that for both reading and maths, the ninth grade results are changed to NaNs. Taking the mean of these results gives us a better understanding of how grade level performances across all schools changed when 





#### Scores by school spending
#### Scores by school size
#### Scores by school type
## Summary
