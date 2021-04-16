# School District Analysis

## Overview

A School District Board recieved an initial analysis of some data they provided.  After reviewing the data they asked to see the analysis without the math and reading grades for the Thomas High School 9th graders.  Thomas High School has 1635 students and 461 are 9th graders.  The School Board has some concern that the information provided in the student data for those students had been altered.  The purpose of this analysis is to see if the findings show any discrepencies.

In the initial analysis the School Board provided the analyst with school and student data for the district.  The school data had the following columns:<br>
__School ID, School Name, Type (of school), Size and Budget.__

The student data consisted of these columns:<br>
__Student ID, Student Name, Gender, Grade, School Name, Reading Score and Math Score__

The initial analysis gathered together information about the schools and students into these summaries:<br>
__District Summary, Per School Summary, Per School Capita, Spending Summary, Summary based on School Size, Summary based on type of School, Top Schools and Bottom Schools, Math Scores by Grade, Reading Scores by Grade__

## Setup for Analysis

This analysis will show through comparision how the initial analysis and the analysis without Thomas High School 9th graders vary.  Here in the output below you can see that the Thomas High School 9th Graders have had their grades removed from analysis by replacing their grades with NaN (Not a number). (Red lines added for emphasis.)

<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/THS_9th_Grade_NaN.png" width="600" height="300" />

## How Results are Calculated

The results in the analysis are looking to see if by removing the grades of the ninth graders from Thomas High School affect the overall percentage of passing students in math and reading.  To run these calculations, per the setup, all 9th grade grades for THS are set to NaN.  Only scores above or equal to 70% are considered passing.  The students who pass is then divided by the total students (district and then school only) and multiplied by 100 to get the percentage of passing in each, math and reading, and in both math and reading.  

## Results

### How the District Summary has been affected

By removing the ninth graders grades for Thomas High School the differences in the percentages are very minimal with overall passing dropping from 65.2% to 64.9%. This minimal drop could be expected since there are 39,170 students in the disctrict and only 461 are 9th graders at THS.  A percentage of the population of only 1.2%. Here are the outputs 

__Initial District Summary__
<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/Initial_District_Summary.png"  />

__THS 9th Graders Grade removed__
<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/District_Summary_wo_9th.png" />


### How the School Summary has been affected

The School Summary below provides a more granular level look at the percentages.  Where above in the district summary the 9th graders were only 1.2% of the overall population, they are now 39.3% of the school population.

Here the analysis is specifically interested in the grades for the Thomas High School and the school summary outputs below show the initial analysis and the refactored analysis when the 9th graders grade were removed.

The % Passing Math, % Passing Reading and the % Overall Passing show clearly that without the 9th graders grades the percentages drop significantly. When the 9th grade scores above 70% in math and reading are removed from the school scores reading drops passing math drops from 93.27% to 66.91% and reading drops from 97.3% to 69.66%.  

Here are the outputs:

__Initial School Summary for Thomas High School__
<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/Per_School_header.png"  />
<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/Initial_Per_School_Summary.png"  />

__School Summary with 9th Graders removed__
<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/Per_School_Summary_w_9th_asNaN.png" />

When Thomas High School scores are calculated on 10th, 11th and 12th graders passing scores only and dividing by 1174 total students which removes 9th graders from the total of 1635 we see that the scores once again go up to close the original output.
__School Summary for 10th, 11th and 12th only__
<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/Per_School_Summary_wo_9th.png" />

### How replacing the ninth grade math and reading scores affected Thomas High School performance relative to other schools

In the initial analysis Thomas High School with it's overall passing percentage above 90% placed it in the top 5 schools in the district.  But when the analysis was done here and the ninth graders percentages were removed Thomas High School moved out of the top 5 because it's overall passing percentage went to 65%.  Here is a look at the Top 5 with 9th graders from THS removed.
<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/Top_Schools_w_9th_NaN.png" />

This is what the Top Schools look like with just Thomas High School 10th, 11th and 12th Graders.  This shows that their grades were good enough to bring them into the top 5 schools.
<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/Top_Schools_wo9th.png" />

The Bottom Schools did not change.
<img src="https://github.com/linb960/School_District_Analysis/blob/main/Resources/Bottom_Schools.png" />


#### Math and Reading scores by grade

#### Scores by school spending

#### Scores by school size

#### Scores by school type

## Summary
Summarize four major changes in the updated school district analysis after reading and math scores for the ninth grade at Thomas High School have been replaced with NaNs.
