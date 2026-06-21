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

### 2. Data Quality Issues

| Issue # | Variable(s) | Issue Type | Description | Status |
|---------|-------------|-----------|-------------|--------|
| 1 | Electorate size, Total Households, MGNREGS Active Job Cards, PM-KISAN Beneficiaries | Outliers | Outliers may exist in these variables based on the range between minimum and maximum values | Requires Validation |
| 2 | Voter Turnout%, Literacy Rate%, Internet 4G Coverage% | Range Validation | Percentage variables are within the valid range of 0-100 | ✓ Valid |
| 3 | All Numerical Columns | Missing Values & Consistency | Dataset should be checked for missing values and consistency before advanced analysis | Requires Validation |

**Overall Assessment:** The dataset appears suitable for analysis with only routine validation checks required.

### 3. Two Derived Columns
   1. BPL Households 
   Formula: ( BPL Household Count/ Total Households)* 100
   Reason : The absolute number of BPL households does not account for difference in constitency size. Converting it into a percentage a better measure of poverty levels and allows meaningful comp[...]
  2. PK-KISAN Coverage rate
     Formula: (PK-KISAN Beneficiaries/ Total Households)*100
     Reason : This Measure the  Proportion of households receiving PM-KISAN benefits. It helps asses the reach of  agricultural welfare support across constituencies and highlights areas where ben[...]

## Section 2:  Analytical Deep- Dive

### 1. Regional Disparities
   To find out the average I have analyzed data from 60 constituencies across Meghalaya to compare  JJM Water Coverage, Road infrastructure, and  Literacy rate for Khasi, Jaintia and Garo Hills regions.
   
Steps i followed :

1. I used the 'AVERAGEIF' function in Excel to calculate the mean for each region.

2.  The data was already in percentage form. So '66.3' means 66.3%.

 Results Table :

| Region | JJM Water Coverage | Road Infrastructure | Literacy Rate |
|--------|-------------------|-------------------|---------------|
| Khasi Hills | 66.30% | 66.70% | 80.30% |
| Jaintia Hills | 50.80% | 51.50% | 74.50% |
| Garo Hills | 45.10% | 56.10% | 72.90% |

Data Analysis: The data shows clear regional disparities. Khasi Hills lead in all three indicators due to the presence of  Shillong, the state Capital and  administrative centre. The biggest gap i in JJM coverage, where Garo Hills at 45.1% is over 20% behind Khasi Hills. However, Garo Hills  has better road infrastructure at 56.1% than Jaintia Hills at 51.5%, despite legging in water and literacy. This suggests uneven development priorities across regions.

