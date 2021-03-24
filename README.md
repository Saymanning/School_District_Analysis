# School_District_Analysis

## Overview

### Original Analysis
The purpose of the original School District Analysis was to provide data on the performance trends of reading and math standardized test data across 15 high schools to The School Board.
The following deliverables were provided in the original analysis:

- A high-level snapshot of the district's key metrics, presented in a table format
- An overview of the key metrics for each school, presented in a table format
- Tables presenting each of the following metrics:
- Top 5 and bottom 5 performing schools, based on the overall passing rate
- The average math score received by students in each grade level at each school
- The average reading score received by students in each grade level at each school
- School performance based on the budget per student
- School performance based on the school size 
- School performance based on the type of school

### Purpose of this analysis:
The School Board discovered that the dataset analyzed, students_complete.csv file shows evidence of academic dishonesty; specifically, reading and math grades for Thomas High School ninth graders appear to have been altered. The school board does not know the full extent of the academic dishonesty, however they want to uphold state-testing standards and asked for the math and reading scores for Thomas High School be replaced with NaNs while keeping the rest of the data intact. After the math and reading scores were replaced with NaNs, the school district analysis was repeated to find if and/or how these changes affected the overall analysis.

  See the image below showing a snippet of how the loc method was used with logical and comparison operators, to retrieve the student count for Thomas High School ninth         graders in the school_data_complete_df DataFrame:
  
  <img width="685" alt="loc_method example" src="https://user-images.githubusercontent.com/78699465/112387339-0464e100-8cc8-11eb-9f7f-e928bb41d776.png">


## Results

- **How is the district summary affected?

  The affect of replacing the ninth grade math and reading scores at Thomas High School with NaN(Null) was very minimal as can be seen in the following images.
  
  The image below shows the results replacing the ninth grade math and reading scores at Thomas High School with NaN(Null):
  
  <img width="726" alt="District_Summary Replaced with NaN" src="https://user-images.githubusercontent.com/78699465/112380144-6836dc00-8cbf-11eb-8080-96dbbcbae557.png">

  This image shows the results from the original analysis:
  
  <img width="743" alt="District_Summary_Original" src="https://user-images.githubusercontent.com/78699465/112380230-8997c800-8cbf-11eb-849d-34f773b23895.png">

- **How is the school summary affected?

  Again, the results had a minimal affect on the school summary since only the scores for Thomas High School were replaced. So, the only school to see any change was Thomas     High School. The data remained unchanged for all other schools. 
  
  Thomas High School Data After Analysis Rerun:
  
  <img width="695" alt="THS_Rerun" src="https://user-images.githubusercontent.com/78699465/112384951-66701700-8cc5-11eb-9b71-cdcbd71eda13.png">

  Thomas High School Data from Original Analysis:
  
  <img width="589" alt="THS_Original" src="https://user-images.githubusercontent.com/78699465/112385327-dc747e00-8cc5-11eb-8456-d3fc3656983e.png">
 

 - **How does replacing the ninth-grade scores affect the following:
 
    -Math and reading scores by grade
    -Scores by school spending
    -Scores by school size
    -Scores by school type
    
    As can be seen in the images of data analysis results below, the difference in results is minimal.
    
    Analysis Rerun:
    
    <img width="554" alt="Scores_by_school_spending" src="https://user-images.githubusercontent.com/78699465/112389069-80f8bf00-8cca-11eb-8763-16afa1f52fe3.png">
    
    Original Analysis:
    
    <img width="541" alt="Original" src="https://user-images.githubusercontent.com/78699465/112389078-85bd7300-8cca-11eb-8f16-136ddf7b2222.png">


## Summary
The affect of replacing the ninth grade math and reading scores at Thomas High School with NaN(Null) was very minimal on the dataset as a whole. The minor changes were as follows: The average math score went from 83.418 to 83.351. Average reading score went from 83.849 to 83.896. The percent passing math went from 93.272 to 93.186. The passing reading percent from 97.309 to 97.019 and overall percent passing from 90.948 to 90.630.
