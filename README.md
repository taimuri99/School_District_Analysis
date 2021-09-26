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

After removing the Thomas High School 9th Grade math and reading results the following changes are observed:
  1) Average Math Score decreases
  2) Average Reading Score remains unchanged
  3) Math Passing Percentage decreases
  4) Reading Passing Percentage decreases
  5) Overall Passing Percentage decreases

### How is the school summary affected?
Below is the original school summary:

<img width="954" alt="Columns heads" src="https://user-images.githubusercontent.com/87828174/134786756-d28a2aff-9367-4151-8cfa-0be577bc3d36.png">
<img width="954" alt="OriginalSchoolSummaryTHS" src="https://user-images.githubusercontent.com/87828174/134785984-27718242-80f7-4a1a-9d88-a463c148f95f.png">


And here is the updated school summary after taking the math, reading and overall scores and passing percentages for grades 10, 11 and 12 and replacing the values in the previous dataframe with them. This was done to mantain academic integrity by not counting the 9th grade results at all and only counting and creating a summary with 10th, 11th and 12th grade results for Thomas High School.

<img width="961" alt="Columns heads" src="https://user-images.githubusercontent.com/87828174/134786756-d28a2aff-9367-4151-8cfa-0be577bc3d36.png">
<img width="961" alt="NewSchoolummary" src="https://user-images.githubusercontent.com/87828174/134785991-e3efc82b-4076-4b18-b23d-8f15b16f137b.png">

Only the results of Thomas High School are included as the rest of the schools had the same results as before and were unchanged. The following changes are observed after removing the 9th Grade results for Thomas High School:
  1) Average Math Score decreases
  2) Average Reading Score increases
  3) Math Passing Percentage decreases
  4) Reading Passing Percentage decreases
  5) Overall Passing Percentage decreases

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?
Here are the top performing schools before the grades were removed from Thomas High School 9th grade:

<img width="993" alt="OriginalTopSchools" src="https://user-images.githubusercontent.com/87828174/134786494-f94fd459-f5c4-493e-a7a3-5978350449d2.png">

And here are the top performing schools after the grades are removed and only 10th, 11th and 12th grade results are considered for Thomas High School:

<img width="990" alt="NewTopSchools" src="https://user-images.githubusercontent.com/87828174/134786513-1083c6a5-72a8-4080-807f-04ae3ffba06a.png">

As you can see the top 5 schools remain the same with Thomas High School still performing well at second place. Although the passing percentages and maths scores have decreased and reading scores increased, the overall performance with respect to other schools remains the same thus sustaining the integrity of the school and district analysis. The bottom 5 schools are unchanged as well.

### How does replacing the ninth-grade scores affect the following?
#### Math and reading scores by grade
Taking the mean of the averages across all schools for math and reading and for each grade gives us a better understanding of how grade level performances across all schools changed when the 9th grade results of Thomas High school are removed.

Here are the original mean math scores per grade level:

<img width="157" alt="AVGOriginalMath" src="https://user-images.githubusercontent.com/87828174/134787356-507e327d-099c-4295-9570-76fd132a36d8.png">

Here are the new updated averages:

<img width="153" alt="AVGNewMath" src="https://user-images.githubusercontent.com/87828174/134787383-63c7364b-f3b1-4f02-a9c8-47f109950cfb.png">

For reading the original averages:

<img width="155" alt="AVGOriginalReading" src="https://user-images.githubusercontent.com/87828174/134787363-d9b7e82c-2c3c-444b-b511-fbdcf80e045a.png">

and the new updated averages for reading:

<img width="155" alt="AVGNEWReading" src="https://user-images.githubusercontent.com/87828174/134787380-9fb6f8a6-b962-433f-882c-26d195a0f72b.png">

The following changes are observed in the overall school averages per grade when the 9th grade results for Thomas High School are considered as NaNs:
  1) 9th grade average math scores across all schools decreases
  2) Rest of the grade averages for maths across all schools remains unchanged
  3) 9th grade average reading scores across all schools decreases
  4) Rest of the grade averages for reading across all schools remains unchanged

#### Scores by school spending
The schools were grouped by spending ranges per student and outputted as a dataframe with average math and reading scores and average passing percentages. This was done to see the performance of schools in the district in relation to spending budget per student. Here is the original school spending dataframe:

<img width="824" alt="OriginalSchoolSpending" src="https://user-images.githubusercontent.com/87828174/134787665-b3c7a3cb-dba7-45d9-ada2-eaa210e4d44e.png">

Here is the updated one:

<img width="825" alt="NewSchoolSpending" src="https://user-images.githubusercontent.com/87828174/134787673-0d5edd83-afff-4686-940e-bc9ae21b0b75.png">

The only change one see the only change is for the group $630 - $644 budget per student as this is the range in which Thomas High school is present in. The other ranges are not affected. The following changes are observed:
  1) Average Math score for the group $630 - $644 budget per student decreases
  2) Average Reading score for the group $630 - $644 budget per student increases
  3) Math Percentage Passing for the group $630 - $644 budget per student decreases
  4) Reading Percentage Passing for the group $630 - $644 budget per student decreases
  5) Overall Percentage Passing for the group $630 - $644 budget per student decreases

#### Scores by school size

The schools were also grouped by school size to see the performance relationship of schools to their size. Here is the original school size dataframe:

<img width="759" alt="OriginalSize" src="https://user-images.githubusercontent.com/87828174/134787750-1a5e2575-2bcc-4a63-936a-a88009ed11d9.png">

and here is the updated one: 

<img width="761" alt="NewSize" src="https://user-images.githubusercontent.com/87828174/134787743-2ce263e5-6dd5-4e6f-9741-4f8a38060c6a.png">

One can see the only change is in the medium size category of 1000 - 2000 students and not any other range. This happens as Thomas High School is in said range of school size. The following changes are observed:
  1) Average Math score for the group 1000 - 2000 students decreases
  2) Average Reading score for the group 1000 - 2000 students increases
  3) Math Percentage Passing for the group 1000 - 2000 students decreases
  4) Reading Percentage Passing for the group 1000 - 2000 students decreases
  5) Overall Percentage Passing for the group 1000 - 2000 students decreases

#### Scores by school type

The schools were also grouped by school type to see the performance relationship of schools to their type. Here is the original school size dataframe:

<img width="712" alt="OriginalSchoolType" src="https://user-images.githubusercontent.com/87828174/134788334-efeceb2f-46af-4cf8-b433-d761ea6f1ed4.png">

and here is the updated one:

<img width="713" alt="NewSchoolType" src="https://user-images.githubusercontent.com/87828174/134788341-e52bf7ea-b7e0-4d38-bbc4-1f24e1754d13.png">

One can see the only change is in the Charter type category not for District type. This happens as Thomas High School is in Charter school type. The following changes are observed:
  1) Average Math score for Charter Type schools decreases
  2) Average Reading score for Charter Type schools increases
  3) Math Percentage Passing for Charter Type schools decreases
  4) Reading Percentage Passing for Charter Type schools decreases
  5) Overall Percentage Passing for Charter Type schools decreases

## Summary
After the reading and math scores for Thomas High School 9th grade have been replaced, the following four changes are observed. The analysis of the school district data according to different paramaters of school type, size, funding budget and in general by schools all follow a similar trend. Average math scores decrease while average reading scores increase. Passing percentages for reading, maths and overall decrease. Another noticeable change is that all average scores and passing percentages for maths and reading across 9th grade for all schools decrease. Lastly in the district summary, the average math score, math passing percentage, reading passing percentage and overall passing percentage decrease. However the average reading score remains the same.
