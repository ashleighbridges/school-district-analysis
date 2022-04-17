# school_district_analysis

## Overview
After completing a full analysis of the PyCity School District's math and reading scores, it was discovered that the Thomas High School 9th grade test scores may have been tampered with and required further investigation. Due to these irregularities, I needed to drop all of the THS 9th grade scores and re-run the analysis without them to report to the school district.

## Results
### District Summary
Removing the THS 9th grade scores created a minor but measurable change in the district summary. As evidenced below, removing the scores:
- Decreased the Average Math Score by 0.1
- Decreased the % Passing Math by 0.2%
- Decreased the % Passing Reading by 0.1%
- Decreased the % Overall Passing by 0.3%

*Original District Summary:*
![PCS_district_df](https://user-images.githubusercontent.com/100883212/163727184-28aa0b94-7a62-4c08-9164-14c21fbcc4b9.png)

*Updated District Summary:*
![Challenge_district_df](https://user-images.githubusercontent.com/100883212/163727202-be4885f6-791e-4dbf-9def-47a0e54ee6e7.png)

### School Summary
As evidenced below, removing the scores for the 9th grade class affected all of the results on the Thomas High School summary, however these two scores had more major differences:
- % Passing Reading decreased by 0.3%
- % Passing Overall decreased by 0.3%

*Original THS School Summary*
![THS_school_summary](https://user-images.githubusercontent.com/100883212/163727834-929d3c9a-b495-4a05-a1b3-8208451b7b7c.png)

*Updated THS School Summary*
![THS_updated_school_summary](https://user-images.githubusercontent.com/100883212/163727843-a4147af0-52c1-47e2-af8d-fa2ef1e008b3.png)

### THS vs. Other Schools
While removing the THS 9th grade class scores did affect their overall school scores, it had negligable difference on how they related to the rest of the district. They are ranked #2 in the district in both the original and updated per school summaries

*Original Top 5 Summary*
![Top_5_summary](https://user-images.githubusercontent.com/100883212/163728169-1cf19a26-85ae-45df-bd73-14ac2295d353.png)


*Updated Top 5 Summary*
![Updated_Top_5_summary](https://user-images.githubusercontent.com/100883212/163728177-00632c1f-89d6-44d3-9b7a-8bb091d6acb7.png)

### Other DataFrames
While there were small differences in the results for the remainder of the DataFrames created for the analysis, formatting (including rounding results to a reasonable number of decimal places) led to no difference showing for the following DataFrames:
- Math and Reading Scores by Grade
- Scores by School Spending
- Scores by School Size
- Scores by School Type

## Summary
While removing the Thomas High School 9th grade scores from the data did have some effects on the results, they were very minimal overall. The few noticable changes included the THS % Passing Reading and % Passing Overall results each decreasing by 0.3% as well as the District Average Math Score decreasing by 0.1, the % Passing Math decreasing by 0.2%, the % Passing Reading decreasing by 0.1%, and the % Overall Passing decreasing by 0.3%. All other DataFrames created had either negligable or no change detected at all.
