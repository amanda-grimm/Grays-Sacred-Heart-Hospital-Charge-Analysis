# Grays-Sacred-Heart-Hospital-Exploratory-Data-Analysis

## EXECUTIVE SUMMARY

This project features an exploratory data analysis for Gray's Sacred Heart (GSH), a maternal health hospital, focused on patient charges. The data for this project was provided for me via Pathstream. I cleaned, wrangled, analyzed, and visualized the data using google sheets. The data was analyzed as a whole, and then further analyzed when broken down into newborn only and mother only. After identifying causes for disparities in charges, I recommend the following changes to keep GSH's cost-to-charge ratio near 50%:

  1. Increase charges for the following newborn procedures by 7-3% ***insert photo here****
  2. Aim for 2-night stays for newborns
  3. Increase charges for self-pay patients by 1-5%
 
 

## BUSINESS PROBLEM
GSH is a non-profit hospital that largely relies on grants for its funding in order to keep the doors open and provide care to mothers and newborns. These grants depend on consistency in charges to the patients, so it is important to analyze the charges in relation to procedures completed in order to ensure consistency is occurring. This analysis happens on a yearly basis in order to ensure the cost-to-charge ratio remains steady despite changes in the cost of providing health care, along with the challenge of keeping healthcare affordable for this population. The chief medical director has requested the following:

  1. Analysis of the data as a whole, and then further independent analysis of mother-only data and newborn-only data
  2. Identify major factors that affect the cost of a patietnt's care
  3. Identify what patients, procedures, or operations are causing patients to be over or under charged


## METHODOLOGY
### DATA WRANGLING
1. Sorted cleaned_data by total charges and compared rows with same costs, cross-referencing with other values like birth weight and attending operating providers.
2. Created a new sheet and used the unique function.
3. Copied and pasted the values from the unique function results.
4. Corrected format of zip code values, i.e. changing (121) to 121.
5. Deleted any rows with OOS in zip code column (4 rows).
6. Changed Male/Female formats to M/F.
7. Changed Admission Type to Newborn for any patient marked M that also had CCS Diagnosis mentioning preinatal jaundice and/or APR DRG listing Neonate birthwt.
8. Separated Payment Typology into 3 separate columns.
9. Split data into a Mothers sheet and a Newborns sheet.

10. ***SIMPLIFY THIS LIST & ADD A SIMLIFIED LIST BELOW FOR EDA

### EXPLORATORY DATA ANALYSIS



SKILLS
Spreadsheets: column splitting, calculated columns, pivot tables, 
