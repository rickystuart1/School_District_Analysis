# School District Analysis

## Purpose
The purpose of this project was to analyze data of a school district by cleaning it and organizing it to show several metrics of each school in the district based off of their student's testing scores. After the initial analysis, information was brought to the district showing that there was a possibility that there could have been academic dishonesty from one of the school's 9th grade class. So a second analysis was performed with the potentially dishonest math and reading scores for the 9th graders being replaced with 'NaN' at Thomas High School. 

## Resources
Data source: students_complete.csv & schools_complete.csv

Software: Python 3, Jupyter Notebook, Pandas, Numpy

## Results
### School District Summary 

- After setting the 9th grade Thomas High School student scores to NaN, the 461 student's scores were not included in the calulations. Because of this:
  - The district average math score decreased by .2 points, while the district average reading score was not changed.
  - The district passing math percentage decreased by .2 percentage points and the district passing reading percentage was decreased by .3 percentage points. 
  - The overall district passing percentage decreased by .1 percentage points. 
<img src="analysis/district_summary_df.png" >

### School Summary 

- In this portion of the analysis, the information is separated by school. So the only row affected by the change was Thomas High School. The changes include:
  - Thomas High School's average math score was unaffected, while the average reading score actually increased by .1 points.
  - Thomas High School's average math passing percentage decreased by .1 percentage points and average passing reading percentage decreased by .3 percentage points. 
  - Thomas High School's overall passing percentage decreased by .3 percentage points. 
<img src="analysis/per_school_summary_df.png" >

### Top Five Schools
- When the 9th grade students scores were removed, their schools overall ranking dropped drastically to 8th overall in the district. But once their scores were calculated for only the 10th - 12th grade students, they regained their position as the second best school in the district. Shown Below:
<img src="analysis/top_schools.png" >

### Bottom Five Schools
<img src="analysis/bottom_schools.png" >

### Average Scores by Schools and Grade Level
- The only affect that was displayed on this table were that the scores for the 9th grade students at Thomas High School were made NaN. All other grade levels and every other school was unaffected. 
#### Average Reading Scores
<img src="analysis/avg_reading_scores.png" >

#### Average Math Scores
<img src="analysis/avg_math_scores.png" >

### Scores by School Spending
- The change had a very insignificant impact on the Scores by School Size table, and could not be seen with the rounded values.
<img src="analysis/student_budget.png" >

### Scores by School Size
- There was also no impact on the Scores by School Size with the rounded values.
<img src="analysis/school_size.png" >

### Scores by School Type
- Like the previous two tables, there was no impact seen on the Scores by School type table. 
<img src="analysis/school_type.png" >


## Summary 
In conclusion, four noticeable take aways could be interpreted after performing the changes to the analysis of the school district. By removing the scores of the potentially academically dishonest 9th grade students from Thomas High School and replacing them with NaN, we could see that:
- The district overall passing percentage was decreased by one tenth of a percentage point. 
- Thomas High School's overall passing percentage decreased by three tenths of a percentage point. 
- When the 9th grade students at Thomas High School's grades were replaced with NaN their passing percentage dropped significantly, forcing them out of the top 5 schools in the district. But when only the 10th-12th grade students were taken into account, they reclaimed their position as the second best school. 
- Overall, replacing the 9th grade Thomas High School student's grades had a very insignificant impact on all of the data, and it is questionable if the second analysis should have been performed.  
