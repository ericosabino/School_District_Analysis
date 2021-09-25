# School District Analysis

## The Analysis and the change
The initial analysis covered the performance of the students and their respective in various dimensions. After it was discovered that the Thomas School students of the 9th grades had their scores altered, the analysis was redone by resetting scores for the 9th grade students to null.

New tables were generated and the comparison between previous analysis and the current one is found below.

# Conclusions

## How is the district summary affected?

In the District summary, we see a small drop on the Average Math Score (79 to 78.9) while the Average Reading Score is the same (81.9).

We can also note a slight drop on the other indicators, % Passing Math came from 75 to 74.8, while the % Passinh Reading went from 86 to 85.7.
The % Overall Passing went from 65 to 64.9.

Here are the tables comparing the data:

### Fig 01. Original District Summary.
![](Images/01_district_summary.png)

### Fig 02. District Summary after removing Thomas School 9th grade students.
![](Images/01_district_summary_new.png)


## How is the school summary affected?

When analyzing the metrics for Thomas High School after removing the 9th grade students scores and their counts, we are able to see an Average Math Score of 83.350937, an Average Reading Score of 83.896082 and an % Overall Passing of 90.630324.

Please note that the total students for 10th to 12th grades is 1175. The figures shows 1635, which is the total students for Thomas High School.

### Fig 03. Thomas High School Summary after removing 9th grade studentsscores and counts.
![](Images/02_school_summary_new.png)


## How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Originally, Thomas High School was placed in the second place in the top 5 schools rank sorted by % Overall Score. As seem on the Fig. 06, removing the grades form the 9th students and changing the count of students kept the school in the same position.

### Fig 04. Original Top 5 Schools
![](Images/03_top_5_schools.png)

### Fig 05. Top 5 Schools without Thomas students
![](Images/03_top_5_schools_new.png)

There we no changes in the bottom 5 high schools, as seen in the figures below:

### Fig 06. Original Bottom 5 Schools
![](Images/04_bottom_5_schools.png)

### Fig 07. Bottom 5 Schools without Thomas students
![](Images/04_bottom_5_schools_new.png)


## How does replacing the ninth-grade scores affect the following:

Below are the comparison of the scores by grade before and after the removal of Thomas High School 9th grade students:

### Fig 08. Comparing Original and modified Math Scores.

Before Removal Math Scores by Grade | After Removal Math Scores by Grade
:-------------------------:|:-------------------------:
![](Images/05_math_scores_by_grade.png)  |  ![](/Images/05_math_scores_by_grade_new.png)


### Fig 09. Comparing Original and modified Reading Scores.
Before Removal Reading Scores by Grade | After Removal Reading Scores by Grade 
:-------------------------:|:-------------------------:
![](Images/06_reading_scores_by_grade.png)  |  ![](/Images/06_reading_scores_by_grade_new.png)


The other factors were also impacted by removing the 9th grade students scores and counts of the analysis.

## Scores by school spending

In terms of spending ranges, the Budget per Student in Thomas High School increased from 638 to 888, what made the school be classified on a separated tier from the other schools.

### Fig 10. Original passing % and averages by Spending Ranges
![](Images/07_score_by_spending_ranges.png)

### Fig 11. Passing % and averages by Spending Ranges after removing Thomas High School 9th grade students.
![](Images/07_score_by_spending_ranges_new.png)


## Scores by school size

When we compare the scores in terms of school size, the numbers were not impacted, as the change in the scores were not significant after removing the 9th grade students and their counts, and the schools is still classified as medium size (the size went from 1635 to 1174, which is still in the range of 1000 ~ 2000).

### Fig 12. Original passing % and averages by School Size
![](Images/08_score_by_school_size.png)

### Fig 13. Passing % and averages by School Size after removing Thomas High School 9th grade students.
![](Images/08_score_by_school_size_new.png)



## Scores by school type
As the analysis by school size, the analysis by school type presented the same values, and for the same reason. The classification hasn't changed and the scores were not significantly affected.

### Fig 14. Original passing % and averages by School Type
![](Images/09_score_by_school_type.png)

### Fig 15. Passing % and averages by School Type after removing Thomas High School 9th grade students.
![](Images/09_score_by_school_type_new.png)


# Change Summary

Many changes needed to be done in the updated school analyis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs. Mainly, these changes were:

1. Recalculating the Average Math Score, Average Reading Score, % Passing Math, % Passing Reading and % Overall Passing considering the count and scores of students from the 10th and 12th grades only.

2. Recalculating the Top 5 schools rank considering scores of students from the 10th and 12th grades only.

3. Replacing the school size for Thomas High School from 1635 to 1174 in the school_data_complete_df and school_data_df DataFrames to complete the Analysis by school spending, school size and school type.

4. Creating a new tier on the bins to include schools with spending ranges per students above 676, as Thomas High School's spending range per student increased from 638 to 888.







