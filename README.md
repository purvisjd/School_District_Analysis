# School District Analysis

## Overview of analysis:
This project began as an evaluation of the academic success of schools within the Py City Schools
district.  This success was determined utilizing the outcome of standardized testing, specifically
the reading and math scores for all 9th through 12th grade students within the district.  During
the course of the evaluation, concerns were raised as to the validity of the scores for the 9th grade
class from Thomas High School.  Adjustments were made to the existing datasets and all scores for the
9th grade class from Thomas High School were removed from the analysis and the outcome recalculated 
to reflect the new numbers
### Resources:
* Data:  students_complete.csv, schools_complete.csv
    *  [Students Complete](https://github.com/purvisjd/School_District_Analysis/blob/main/Resources/students_complete.csv)
    *  [Schools_Complete](https://github.com/purvisjd/School_District_Analysis/blob/main/Resources/schools_complete.csv)
*  Software:  Anaconda, Jupyter Notebook 6.3.0

##  Results of Analysis:
Due to concerns about the potential for academic dishonesty, adjustments had to be madeand the analysis re-run for the district.
To remove the potential of skewed results attributable to dishonesty, all reading and math scores for the 9th grade class at Thomas High School
were changed to NaN within the dataframes so as to not have them counted in some of the calculations.  This would, obviously,
have some impact on the numbers from the previously run analysis:
*  How is the district summary affected?
    *  For the initial analysis, the district summary was calculated as:
      ![image](https://user-images.githubusercontent.com/85641017/126503839-bcb9db3c-1b14-4805-9c33-a5d9a87bdc2b.png)
    *  Once the adjustments to the 9th grade scores were made, the district summary now
       shows as:
       ![image](https://user-images.githubusercontent.com/85641017/126503962-8c443d6a-3763-4899-ab77-93fd9f7edf34.png)
    *  The total budget would not be affected by the changes since that total was based on the amount spent on each student regardless of the overall scores.
    *  The total number of students would also remain the same as part of the analysis is a reflection of all of the identified students within the district regardless of score outcomes.
*  How is the school summary affected?
    *  The impact of the update on the school summary is also minimal as shown below.  The differences between previous outcomes and updated outcomes are less than 1/2 a point.
    	                
                           Average Math   Average Reading    % Math     % Reading    % Overall
              Original     83.418349       83.84893          93.272171  97.308869    90.948012
             
             Updated       83.350937       83.896083         93.18569   97.018739    90.630324

*  There would be no impact on the budget and total students as, again, those numbers are sepaate from the academic success markers.
*  How does replacing the ninth graders' math and reading scores affect Thomas High School's performance relative to other schools?
    *  When the school totals are run and sorted by % Overall Passing as they had been done in the original analysis, there is no impact on Thomas High School's performance.   They remain with the second highest overall passing rate with 90.630324% passing:
    
    ![image](https://user-images.githubusercontent.com/85641017/126506149-ace4192b-dc46-4046-a8ab-453350c515ab.png)
*  How does replacing the ninth-graders scores affect the following:
    *  Math and reading scores by grade
        *  Replacing the 9th grader scores removes all entries for Thomas High School for that category.  When the two data frames are produced, Thomas High School's entry for both shows "nan" and it does not contribute numbers towards the overall categories:
        
        ![image](https://user-images.githubusercontent.com/85641017/126506967-5077c06a-48b1-4e42-a840-0dda7f9c91c3.png)
        ![image](https://user-images.githubusercontent.com/85641017/126506993-726fe918-b518-4134-beb6-232f0767a306.png)
        *  Scores by School Spending, Scores by School Size, and Scores by School Type are all going to reflect the same minimal overall impact by removing the 9th grade scores for Thomas High School.  The impact on the overall numbers did not have a significant enough impact to change their relative position on the respective lists nor did it have any impact on the school's overall size nor type.

##  Summary:
Miimal overall changes were observed with the updated 9th grade scores for Thomas High School.  The average math score, as well as the % passing, were lowered minimally, but the reading scores weree not perceptibly changed.  Thomas High School remains a high performer for the district regardless of these changes which is indicative of a strong overall quality to the school.  The district summary also reflects a .1% decrease in the overall passing percentage as a result of no longer including the Thomas HS scores.   The individual scores for the school are lowered as a result of the updated analysis, but again, the changes are minimal given the level of accuracy and formatting used.  Overall, Thomas High School remains a top performer for the district regardless of the potential academic scandal.


