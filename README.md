# BMI_Analysis

![](BMIn.png)
---
# Introduction
BMI is a measure used to determine health using weight and height. This project was done to analyze the BMI of individuals.


_**Disclaimer:** This dataset isn't associated with any health organization, therefore, the validity isn't trusted. It is purely for learning and practicing purposes._

# Problem Statement
1. Distribution of gender in the dataset?
2. Age distribution of the individuals?
3. How does BMI correlate with age and gender?
4. How many individuals fall into the different BMI classifications?

# Tools Used
- Miscrosoft excel was used for data cleaning and preparation.
- Power BI was used for visualization.

## Data Cleaning and Preparation
- There were no duplicate values.
- Handling blank cells: There were a lot of blank cells. For rows with available weight and height values but missing bmi values, the BMI was calculated using the formula
`(weight/(height*height))*703`. While rows with missing values for either weight and BMI, height and BMI, or all three vital values were removed as their presence would negatively impact the analysis.
- BMI Classification: Using the range given by [CDC](https://www.cdc.gov/healthyweight/assessing/index.html#:~:text=If%20your%20BMI%20is%2018.5,falls%20within%20the%20obese%20range.),
I classified the BMI outcome into Underweight, Healthy Weight, Overweight, and Obese, with the IF formula `=IF(G2>=30,"Obese",IF(G2>=25,"Overweight",IF(G2>=18.5,"Healthy Weight","Underweight")))`
- Age group: `=IF(B2>=31,"31-35",IF(B2>=26,"26-30",IF(B2>=22,"22-25","18-21")))`

## Visualization
(Dashboard)

# Insights
1. Out of 24,967 individuals, none fell under the Obese classification, and only 6 were Overweight. The majority of both males and females fell into the Healthy Weight classification leaving a total of 7,401 Underweight.
2. There is no strong relationship between height, weight and age. This shows that a person's age or height doesn't necessarily influence their weight.
3. Majority of the individuals within the 31-35 age group have a healthy weight.

_Use this [BMI Calculator](https://incomparable-tanuki-d71592.netlify.app/), developed by Richard, to check your BMI._


