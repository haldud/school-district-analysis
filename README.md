# School District Analysis
We have been analyzing high school students' performance in math and reading across one district. There are two data sets that we have been given:
1. The first data set contains the list of high schools and various attributes such as type, size, and budget:
   [High Schools](https://github.com/haldud/school-district-analysis/blob/a3d2a825774e48140607f5e16822f9cd211d3a30/Resources/schools_complete.csv)
2. The second data set contains all of the unique high school students in the district along with their math and reading scores.
   [Students](https://github.com/haldud/school-district-analysis/blob/a3d2a825774e48140607f5e16822f9cd211d3a30/Resources/students_complete.csv)
   
Throughout the module, we worked on ensuring that the data sets had complete and usable data to analyze properly. The complete code and analysis can be found in the [PyCitySchool](https://github.com/haldud/school-district-analysis/blob/a3d2a825774e48140607f5e16822f9cd211d3a30/PyCitySchools.ipynb) Jupiter Notebook file. We performed analysis to determine some of the following:
- average math and reading scores
- % of students passing
- per student budget by school
- passing percentages by grade
- performance by budget per student
- performance by school size
- performance by school type (charter or district)

## Overview
For our challenge, we were given information that there was academic dishonesty, and that we needed to exclude all math and reading scores for 9th grade students at Thomas High School. We will be repeating the same analysis as we had done previously after clearing out all math and reading scores for those students. We will be comparing the new analysis to our original to understand how excluding the 9th grade scores of Thomas High School affected our results. The code and results are located in the [Challenge](https://github.com/haldud/school-district-analysis/blob/3fab0f6403ad34d2ed33ee771adc7395ae944220/PyCitySchools_Challenge.ipynb) file.

## Results
Let's analyze the differences in detail for the seven school district metrics that were calculated:
1. District Summary - slight changes were determined for the following
   - Average Math Score dropped from 79.0 to 78.9
   - % Passing Math dropped from 75.0 to 74.8
   - % Passing Reading dropped from 86.0 to 85.7
   - % Overall Passing dropped from 65.0 to 64.9
2. School Summary - slight changes were determined for the following
   - Average Math Score dropped from 83.418349 to 83.350937
   - Average Reading Score rose from 83.848930 to 83.896082
   - % Passing Math dropped from 93.272171 to 93.185690
   - % Passing Reading dropped from 97.308869 to 97.018739
   - % Overall Passing dropped from 90.948012 to 90.630324
3. High and Low Performing Schools - unaffected
   - Thomas High School stayed second on the list of high performing schools
4. Math and Reading Scores by Grade - unaffected except for the following due to removal of scores
   - Thomas High School 9th grade math changed from 83.6 to NaN (or empty) 
   - Thomas High School 9th grade reading changed from 83.7 to NaN (or empty) 
5. Scores by School Spending
   - Thomas High School was in the $630-644 bin and the removal of scores did not affect any of the numbers
6. Scores by School Size
   - Thomas High School is a Medium sized school and the removal of scores did not affect any of the numbers
7. Scores by School Type
   - Thomas High School is a Charter school and the removal of scores did not affect any of the numbers

## Summary
Overall, the removal of the math and reading scores did not have a significant impact. Diving into the district summary statistics and focusing on the scores that changed, the largest observed drop was no more than 0.3% (% Passing Reading). Additionally, the Average Math Score dropped 0.1%, the % Passing Math dropped 0.2%, and the % Overall Passing dropped by 0.1%. It was important to re-run the analysis to ensure the changes were not more significant. Even though the changes were not drastic, removing the scores in question was the right to do to ensure that the state is receiving as accurate data as possible.
