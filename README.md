# School_District_Analysis

## Overview of the School District Analyis
The academic board for the PyCity School District is under the impression that some students in the district engaged in academic dishonesty. More specifically, Maria's supervisor and the board believe that 9th graders at Thomas High School altered their reading and math scores. The board wants Maria to reconduct the analysis, but replacing the 9th grade scores with Nans. The original analysis can be found [here](https://github.com/jackogross123/School_District_Analysis/blob/main/PyCitySchools.ipynb) and the completed challenge analysis can be found [here](https://github.com/jackogross123/School_District_Analysis/blob/main/PyCitySchools_Challenge.ipynb). In the challenge, the board wanted Maria to find:
- The district summary
- The school summary
- The top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score for each grade level from each school
- The average reading score for each grade level from each school
- The scores by school spending per student, by school size, and by school type

## Results
### Analyis Resource 
- Data Sources: [schools_complete](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/schools_complete.csv), [students_complete](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/students_complete.csv), [missing_grades](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/missing_grades.csv), and [clean_students_complete](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/clean_students_complete.csv).
- Software: Juptyer Notebook 6.1.4, Python 3.7.6

### How is the district summary affected?

Original Analysis
![district_summary_OG](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/district_summary_OG.png)

New Analysis
![district_summary_NEW](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/district_summary_NEW.png)

#### Findings
There were not many take aways from replacing the 9th grade scores with Nans. As it can be seen from the two dataframes, there was only a slight decrease in the percentage of students passing in the new analysis. Average math scores stayed the same and average reading scores only dropped by 0.2.

### How is the school summary affected?

Original Analysis
![per_school_summary_OG](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/per_school_summary_OG.png)

New Analysis
![per_school_summary_NEW](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/per_school_summary_NEW.png)

#### Findings
Because of our code, the only school that was affected by the new analysis was Thomas High School. Since only the 9th graders at Thomas High School were accused of academic misconduct, they're the only section that is altered.  

### How does replacing the ninth graders’ math and reading scores affect Thomas High School’s performance relative to the other schools?

Original Analysis
![Thomas_HS_OG](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/Thomas_HS_OG.png)

New Analysis
![Thomas_HS_NEW](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/Thomas_HS_NEW.png)

#### Findings
As it can be seen from the these two graphics, the Thomas High School summaries were dramatically changed by replacing the 9th grade scores with NaNs. While average math and reading scores did not fluctuate greatly, the % of students passing dropped significantly. The % of students passing dropped from 90.94% to 65.07%. At the same time % passing math and % passing reading dropped from 93.27% to 66.91% and 97.3% to 69.66%.

### How does replacing the ninth-grade scores affect the following:
#### Math and reading scores by grade
#### Scores by school spending
#### Scores by school size
#### Scores by school types


## Summary
