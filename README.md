# MlRF-Assignment-
MlRF Assignment Submission 

## Section 1: Data Audit

### 1 Summary Statistics

**Numerical Columns (8):**
1. Electorate size
2. Voter Turnout%
3. Total Households
4. BPL Household Count
5. MGNREGS Active Job Cards
6. PM-KISAN Beneficiaries
7. Literacy Rate%
8. Internet 4G Coverage%

| Variable | Mean | Median | Minimum | Maximum | Std Dev |
|----------|------|--------|---------|---------|---------|
| Electorate size | 29802.10 | 24903 | 11305 | 63978 | 14981.12 |
| Voter Turnout% | 77.88 | 78.9 | 55.5 | 91.1 | 8.84 |
| Total Households | 4340.02 | 3429 | 1629 | 11211 | 2313.39 |
| BPL Household Count | 1485.81 | 1337 | 491 | 2892 | 523.58 |
| MGNREGS Active Job Cards | 835.58 | 846 | 120 | 1987 | 412.04 |
| PM-KISAN Beneficiaries | 744.63 | 732 | 176 | 1634 | 337.32 |
| Literacy Rate% | 75.83 | 75.7 | 58.7 | 95.3 | 10.09 |
| Internet 4G Coverage% | 51.92 | 45.5 | 18.1 | 96.9 | 21.56 |

### 2. Data Quality Issue
After reviewing the dataset, the following are the data quality issues were observed:
. Outliers may exist in variables such as electorate size,total households, MGNREGS Active Job Cards and PM-KISAN beneficiaries.
. Percentage variables such as Voter Turnout, Literacy Rate, and Internet 4G Coverage are all within the valid range of 0-100.
. The Dataset should still be checked for missing values and consistency before advanced analysis.
Therefore, the dataset appears suitable for analysis with ony routine validation checks required.

### 3. Two Derived Columns
   1. BPL Households 
   Formula: ( BPL Household Count/ Total Households)* 100
   Reason : The absolute number of BPL households does not account for difference in constitency size. Converting it into a percentage a better measure of poverty levels and allows meaningful comparison across constituencies.
  2. PK-KISAN Coverage rate
     Formula: (PK-KISAN Beneficiaries/ Total Households)*100
     Reason : This Measure the  Proportion of households receiving PM-KISAN benefits. It helps asses the reach of  agricultural welfare support across constituencies and highlights areas where beneficiary coverage may be relatively low.
