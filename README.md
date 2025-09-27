# Grays-Sacred-Heart-Hospital-Exploratory-Data-Analysis

## EXECUTIVE SUMMARY

This project features an exploratory data analysis for Gray's Sacred Heart (GSH), a maternal health hospital, focused on patient charges. The data for this project was provided for me via Pathstream. I cleaned, wrangled, analyzed, and visualized the data using google sheets. The data was analyzed as a whole, and then further analyzed when broken down into newborn only and mother only. After identifying causes for disparities in charges, I recommend the following changes to keep GSH's cost-to-charge ratio near 50%:

  1. Increase charges for the following newborn procedures by 7-3% (those in red)
<img width="517" height="462" alt="newborn procedures only" src="https://github.com/user-attachments/assets/80e1c5a2-e172-4d42-a9d3-a72bed0586e2" />

  2. Aim for 2-night stays for newborns
  3. Increase charges for self-pay patients by 1-5%
 
 

## BUSINESS PROBLEM
GSH is a non-profit hospital that largely relies on grants for its funding in order to keep the doors open and provide care to mothers and newborns. These grants depend on consistency in charges to the patients, so it is important to analyze the charges in relation to procedures completed in order to ensure consistency is occurring. This analysis happens on a yearly basis in order to ensure the cost-to-charge ratio remains steady despite changes in the cost of providing health care, along with the challenge of keeping healthcare affordable for this population. The chief medical director has requested the following:

  1. Analysis of the data as a whole, and then further independent analysis of mother-only data and newborn-only data
  2. Identify major factors that affect the cost of a patietnt's care
  3. Identify what patients, procedures, or operations are causing patients to be over or under charged


## METHODOLOGY
### DATA WRANGLING
1. Deleted all duplicated rows.
2. Corrected format of zip code values, i.e. changing (121) to 121.
3. Deleted any rows with OOS in zip code column (4 rows).
4. Changed Male/Female formats to M/F.
5. Changed Admission Type to Newborn for any patient marked M that also had CCS Diagnosis mentioning preinatal jaundice and/or APR DRG listing Neonate birthwt.
6. Separated Payment Typology into 3 separate columns.
7. Split data into a Mothers sheet and a Newborns sheet.

### EXPLORATORY DATA ANALYSIS
1. Created calculated rows for cost-to-charge ratio in each sheet. This metric is the main focus of my analysis in order to answer the business problem.
2. Created pivot tables to explore relationships. This included comparing Sum of Total Cost, Sum of Total Charge, Average Revenue, and Average Cost-to-Charge Ratio when data was sorted by Count of CCS Procedures, Payment Typology, Type of Procedure, Length of Stay, and Zip Code. These comparisons were broken down by mothers only, newborns only, and all together.
3. Created visualizations (histograms and scatter plots) to see distributions of data within these relationships and identify outliers and notable observations.
4. Revisited areas to analyze further, including Severity of Illness and Medical vs Surgical Descriptions.

## SKILLS
Spreadsheets: column splitting, calculated columns, pivot tables, histograms, scatter plots
Analysis: identifying most important variables, revisiting information to explore further, identifying notable findings

## RESULTS & RECOMMENDATIONS
The data showed several areas where the cost-to-charge ratio falls below 50%. The separation of mothers-only and newborn-only data was imperative here, as there were stark differences betweeen the two in areas where improvements are recommended. The business recommendations are as follows:

1. Six out of eleven types of procedures provided to newborns resulted in cost to charge ratios below 50%, ranging between  43% and 47%. GSH should increase the amount they charge for these procedures to meet the 50% cost to charge ratio goal.
   <img width="570" height="331" alt="newborn procedures" src="https://github.com/user-attachments/assets/c4870298-6dbe-4d1d-a515-fd50f078d50d" />


3. When newborns have stays lasting 1, 3, 4, 5, 6, or 7 nights, their average cost to charge ratio drops below 50%, ranging between 46% and 49%. This indicates that overall, GSH is not charging enough for their services, specifically for newborns. GSH should increase their charging rate for newborns by 1-4% and/or aim for a 2-night stay when possible.
   <img width="459" height="290" alt="newborn length of stay" src="https://github.com/user-attachments/assets/aff21676-799e-446a-a0d4-49823d0a684f" />



5. When a patient's pay type is classified as self-pay, their cost to charge ratio generally drops below 50% (45% for mothers only, 50% for newborns only, 49% for both groups combined). When looking at only newborns, this ratio drops below 50% when their pay type is through medicaid or a private health insurance. GSH should identify if their contracts with these organizations indicate a lower reimbursement rate and increase the amount charged for these patients by 1-5%.
   <img width="354" height="427" alt="payment typology" src="https://github.com/user-attachments/assets/097999b0-901b-4309-8764-7007942fc014" />


## NEXT STEPS
1. Create a live dashboard that updates this information regularly and is available to administrators to make decisions on throughout the year.
2. Analyze contracts with insurance providers and re-negotiate reimbursements rate where possible.
