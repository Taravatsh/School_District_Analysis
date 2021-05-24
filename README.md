# School District Analysis

## Overview of Project

Maria, who is the chief data scientist for a city school district, is tasked with the preparation and analysis of all standardized test and providing insights about school performance. As a result, Maria was assisted with the analysis of data on students' funding and standardized test scores, thus aggregating the data and show casing trends in school performance.

### Purpose

The purpose of this project is to further assist Maria in conducting the school district analysis once again due to potential academic dishonesty that was detected by the school board in reading and math grades of Thomas High School ninth graders. As a result of this two technical analysis has to be performed with the use of python script, Pandas library and Jupyter notebook to help the school board in finalizing and reconsidering their decisions regarding school budgets and priorities. These two analysis to be carried are as follows:

1. Replacing the math and reading scores for Thomas High School with NaNs.
2. Repeating the school district analysis.

## Results

This section of the report focuses on how replacing the math and reading scores for Thomas High School affected the analysis of the school district. 

### District Summary

Replacing the math and reading grades of Thomas High School ninth graders' with NaNs within the student data dataframe had a slight affect on the average math score, passing math, passing reading and overall passing percentages among the 15 high schools comparing to the original district summary achieved earlier. This was expected as the total number of students of **39,170** was not changed and the same student count was utilized when calculating the passing rates of both math and reading. The district summary of the initial district anaylsis and the district summary after replacing the math and reading scores of ninth graders' with NaNs are shown in the images below respectively.

 The following changes are seen in the updated district summary dataframe:

- The average math score dropped from **79%** to **78.9%**.
- The average reading score remained the same.
- Passing math percentage dropped from **75%** to **74.8%**.
- Passing reading percentage dropped from **86%** to **85.7%**.
- Lastly, the overall passing percentage dropped from **65%** to **64.9%**.

*Original district summary with math and reading scores of Thomas High School ninth graders:*

![Original district summary](Resources/Original_district_summary.png)


*Updated district summary after excluding the math and reading scores of Thomas High School ninth graders:*

![Repeated district summary](Resources/Repeated_district_summary.png)

### School Summary

Initially when the ninth graders of Thomas High School math and reading scores were replaced with NaNs, affected the passing math, reading and the overall percentages and dropped them to the 60th percentiles. This was predicted and considered misleading since the math and reading scores of ninth graders' were removed but the number of students were kept the same which resulted in a great precentage drop for Thomas high School since approximately quarter of students did not have grades but were still considered among the total student counts in the denominator. Figure below shows the district summary only after removing the math and reading scores of Thomas High School ninth graders while keeping the total student count. 

However, after cleaning the data and taking out the ninth garders number of students count and recalculating the percentages only for tenth to twelfth graders of Thomas Hign School, the percentages increased significantly back to the 90th percentiles similar to the original district summary with negligibly small differences in the scores and percentages. 

**Original per school summary with math and reading scores of Thomas High School ninth graders**

![Original per school summary](Resources/Original_per_school_summary.png)

**Updated per school summary without ninth grade students from Thomas High School**

![Repeated per school summary](Resources/Per_school_summary.png)

As shown in the figures above, the following changes can be seen for Thomas High School:

- The average math score decreased by **0.07%**.
- The average reading score increased by **0.05%**.
- The passing math percentage dropped by **0.08%**.
- The passing reading percentage dropped by **0.3%**.
- The overall passing percentage dropped by **0.3%**.

### Thomas High School Performance

Thomas High School performance performance was not affected as their passing percentages were still within the 90 percentile allowing them to maintain their position among the top five perminmg schools ranked as the second best similar to the original school district analysis performed initially.

*Top five perfoming schools of the original school district analysis with:*

![Original top five schools](Resources/Original_top_schools.png)


*Top five perfoming schools without ninth grade students from Thomas High School:*

![Repeated top five schools](Resources/Top_schools.png)

### Math and Reading Scores by Grade

Replacing the ninth-grade scores of Thomas High School with NaNs only affected the ninth graders math and reading score of Thomas High School with an obvious substituion of NaNs while the math and reading scores of the 10-12th graders remained intact. 

- **Math Scores by Grade**

The math scores by grade level of each school is illustarted in figures below both before and after replacing the ninth-grade scores of Thomas High School with NaNs. As it can be seen the math scores of Thomas High Schools ninth graders were subsituted with NaNs where it previously was **83.6** and the math scores by grade were remain the same for all the remaining schools.

*Math scores by grade level from the original dataset analysis before replacing them by NaNs for ninth graders of Thomas High School:*

![Original math scores by grade](Resources/Original_math_scores_by_grade.png)

*Math scores by grade level from the original dataset analysis after replacing them by NaNs for ninth graders of Thomas High School:*

![Repeated math scores by grade](Resources/Math_scores_by_grade.png)

- **Reading Scores by Grade**

Similarly, the reading scores by grade level of each school is displayed in figures below both before and after replacing the ninth-grade scores of Thomas High School with NaNs. As it can be seen the reading scores of Thomas High Schools ninth graders were subsituted with NaNs where it previously was **83.7**, additionally, the reading scores by grade were remain unchanged for all the remaining schools.

*Reading scores by grade level from the original dataset analysis before replacing them by NaNs for ninth graders of Thomas High School:*

![Original reading scores by grade](Resources/original_reading_scores_by_grade.png)

*Reading scores by grade level from the original dataset analysis after replacing them by NaNs for ninth graders of Thomas High School:*

![Repeated reading scores by grade](Resources/Reading_scores_by_grade.png)


### Scores by School Spending

The average math and reading scores, as well as the passing math, reading and overall percentages by school spending for $630-644 bin where Thomas High School belongs to is remained the same after replacing the math and reading scores of the Thomas High School ninth graders with NaNs as shown in the figures below. Additionally, the scores and percentages for the remianing bins were not affected since the spending per students as well as the school budget did not depend on the cetain grade scores of students.

*Spending summary dataframe with math and reading scores of Thomas High School ninth graders:*

![Original scores by school spending](Resources/Original_scores_by_school_spending.png)

*Spending summary dataframe after excluding the math and reading scores of Thomas High School ninth graders:*

![Repeated scores by school spending](Resources/Scores_by_school_spending.png)

### Scores by School Size

The scores and percentages in terms of average math score, average reading score, passing math and reading scores, as well as the overall passing percentage remained the same for the medium school size bin where Thomas High School is categorized into after replacing the math and reading scores of their ninth graders' with NaNs, as shown in the size summary dataframes before and after excluding reading and math scores of ninth graders. Additionally, the scores and percentages by school size of the remaining bins were not affected as well.

*Size summary dataframe with math and reading scores of Thomas High School ninth graders:*

![Original scores by school size](Resources/Original_scores_by_school_size.png)

*Size summary dataframe after excluding the math and reading scores of Thomas High School ninth graders:*

![Repeated scores by school size](Resources/Scores_by_school_size.png)

### Scores by School Type

Replacing the math and reading scores of ninth graders of Thomas High School with NaNs did not have an impact on the average scores and passing percentages of the charter school type where Thomas High School is categorized. Additionally, the scores and percentages per district school type bin also remained intact.

*Type summary dataframe with math and reading scores of Thomas High School ninth graders:*

![Original scores by school type](Resources/Original_scores_by_school_type.png)

*Type summary dataframe after excluding the math and reading scores of Thomas High School ninth graders:*

![Repeated scores by school type](Resources/Scores_by_school_type.png)

## Summary

After replacing the math and reading scores for the ninth grade at Thomas High School with NaNs, few changes were observed in the updated school district analysis. In the district summary, it was seen that the passing math score was decreased by **0.1%**, the passing math percentage dropped by **0.2%**, the passing reading percentage dropped by **0.3%** and this lead to an overall passing percentage decrease of **0.1%**.  




