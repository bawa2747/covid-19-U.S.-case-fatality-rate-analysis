# Covid-19 U.S. Case Fatality Rate Analysis
Exploratory data analysis of the U.S. Covid-19 case fatality rates by state using the Johns Hopkins CSSE data set from February 2020 to March 2023, visualizing the overall trend, and using multiple linear regression to find factors that predict a state's case fatality rate (CFR).

## Key Findings
- CFRs started out high and dropped, likely due to testing, treatments, and improvement of vaccination rates
- Population density was a **statistically significant** predictor of a state's CFR
- However, it only explained about **19%** of the variation in CFR, suggesting the remaining 81% of the CFR variation could be affected by variables such as a state's healthcare resources, age and race demographics, and vaccination rates that were not included in the model.
  
## Methods
**Libraries used**
- tidyverse
- lubridate
- knitr
- usmap
  
**Workflow**
- Data cleaning, transformation, and EDA in R (tidyverse)
- Visualizations of the U.S. national CFR trends and state CFR vs. state population density
- Multiple linear regression model used to identify predictors of state CFR

Full analysis and code: [COVID-19_US_CFR_Analysis.Rmd](COVID-19_US_CFR_Analysis.Rmd)

## Files
`COVID-19_US_CFR_Analysis.Rmd`: source code and full analysis
`COVID-19_US_CFR_Analysis.pdf`: knitted R Markdown report with visualizations

## Data Source
[Johns Hopkins CSSE COVID-19 Data Repository](https://github.com/CSSEGISandData/COVID-19), licensed under CC BY 4.0
- `time_series_covid19_confirmed_US.csv`: confirmed cases by state and county
- `time_series_covid19_deaths_US.csv`: cumulative count of confirmed deaths and total resident population of each county
