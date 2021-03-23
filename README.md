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

Math scores by grade original analysis
![Math_scores_by_grade_OG](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/math_scores_by_grade_OG.png)

Reading scores by grade original analysis
![Reading_scores_by_grade_OG](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/reading_scores_by_grade_OG.png)

Math scores by grade new analysis
![Math_scores_by_grade_NEW](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/Math_scores_by_grade_NEW.png)

Reading scores by grade new analysis
![Reading_scores_by_grade_NEW](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/Reading_scores_by_grade_NEW.png)

##### Findings
As it can be seen from the 4 graphics, the only thing that changed from the two analyses is that the math and reading scores from Thomas High School 9th graders was replaced with NaNs values. This is because of our filtering of the students. 

#### Scores by school spending

Scores by school spending original analysis
![school_spending_OG](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/school_spending_OG.png)

Scores by school spending new analysis
![school_spending_NEW](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/School_spending_NEW.png)

##### Findings
One analysis that changed from the original analysis is the student scores by school spending dataframe. As it can be seen from the two graphics, the only row that was changed is the $630-644 spending row. This is because Thomas High School falls into that spending bin. Overall passing dropped from 63% to 56% and math and reading passing percentages dropped from 73% to 67% and 84% to 77%.

#### Scores by school size

Scores by school size original analysis
![School_size_OG](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/School_size_OG.png)

Scores by school size new analysis
![School_size_NEW](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/School_size_NWQ.png)

##### Findings
Scores by school size only changed for the medium size school bin. The % of overall passing students dropped from 90% to 85%. 

#### Scores by school types

Scores by school type original analysis
![School_type_OG](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/School_type_OG.png)

Scores by school type new analysis
![School_type_NEW](https://github.com/jackogross123/School_District_Analysis/blob/main/Resources/School_type_NEW.png)

##### Findings
Scoes by school type were affected in the Charter column. Overall passing percentage for charter schools dropped from 90% to 87%.

## Summary
Once the scores were replaced with NaNs the percentage of passing students in math, reading, and overall all dropped considerably. The score averages remained intact. This took Thomas High School down into the bottom five of school rankings. At the same time, this also brought the passing averages for charter schools, medium size schools, and $630-644 spending schools down. This is because Thomas High School has all of those characteristics.
