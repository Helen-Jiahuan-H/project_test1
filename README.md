# project_test1
# Self-Reported Health Analysis

## Project Overview
This project will focus on using public data to explore the significance of “self-reported health” as a health indicator.

## Data Source
1. **NHANES Survey Data**: [1999-2000 Survey Data](https://wwwn.cdc.gov/Nchs/Nhanes/1999-2000/DEMO.XPT)
2. **NHANES Mortality Follow-up Data**: [Linked Mortality Data](https://ftp.cdc.gov/pub/HEALTH_STATISTICS/NCHS/datalinkage/linked_mortality/NHANES_1999_2000_MORT_2019_PUBLIC.dat)
   
## Protocols

- Step 1) Import the dataset
  * Survey Data
     * Import the survey data from the 1999-2000 National Health and Nutrition Examination Survey (NHANES):
    ```stata
       import sasxport5 "https://wwwn.cdc.gov/Nchs/Nhanes/1999-2000/DEMO.XPT", clear
   * Mortality Follow-up Data
      * Obtain follow-up mortality data to analyze over a 20-year period from the National Center for Health Statistics (NCHS). 
   ```stata
   //data
   global mort_1999_2000 https://ftp.cdc.gov/pub/HEALTH_STATISTICS/NCHS/datalinkage/linked_mortality/NHANES_1999_2000_MORT_2019_PUBLIC.dat
   //code
   cat https://ftp.cdc.gov/pub/HEALTH_STATISTICS/NCHS/datalinkage/linked_mortality/Stata_ReadInProgramAllSurveys.do
