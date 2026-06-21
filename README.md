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

1. **Electorate size, Total Households, MGNREGS Active Job Cards, PM-KISAN Beneficiaries** - Outliers
   - Outliers may exist in these variables based on the range between minimum and maximum values
   - Status: Requires Validation

2. **Voter Turnout%, Literacy Rate%, Internet 4G Coverage%** - Range Validation
   - Percentage variables are within the valid range of 0-100
   - Status: ✓ Valid

3. **All Numerical Columns** - Missing Values & Consistency
   - Dataset should be checked for missing values and consistency before advanced analysis
   - Status: Requires Validation

**Overall Assessment:** The dataset appears suitable for analysis with only routine validation checks required.

### 3. Two Derived Columns
   1. BPL Households 
   Formula: ( BPL Household Count/ Total Households)* 100
   Reason : The absolute number of BPL households does not account for difference in constitency size. Converting it into a percentage a better measure of poverty levels and allows meaningful comp[...[...]
  2. PK-KISAN Coverage rate
     Formula: (PK-KISAN Beneficiaries/ Total Households)*100
     Reason : This Measure the  Proportion of households receiving PM-KISAN benefits. It helps asses the reach of  agricultural welfare support across constituencies and highlights areas where ben[...[...]

## Section 2:  Analytical Deep- Dive

### 1. Regional Disparities
   To find out the average I have analyzed data from 60 constituencies across Meghalaya to compare  JJM Water Coverage, Road infrastructure, and  Literacy rate for Khasi, Jaintia and Garo Hills region.
   
Steps i followed :

1. I used the 'AVERAGEIF' function in Excel to calculate the mean for each region.

2.  The data was already in percentage form. So '66.3' means 66.3%.

 Results Table :

| Region | JJM Water Coverage | Road Infrastructure | Literacy Rate |
|--------|-------------------|-------------------|---------------|
| Khasi Hills | 66.30% | 66.70% | 80.30% |
| Jaintia Hills | 50.80% | 51.50% | 74.50% |
| Garo Hills | 45.10% | 56.10% | 72.90% |

Data Analysis: The data shows clear regional disparities. Khasi Hills lead in all three indicators due to the presence of  Shillong, the state Capital and  administrative centre. The biggest gap i in JJM Coverage, where garo Hills at 45.1% is over 20% behind Khasi Hills. However, Garo Hills has better road infrastructure at 56.1% than Jaintia Hills at 51.5%, despite lagging in water and  literacy. This suggest uneven development priorities across regions.

### Section 2 Q2: Scheme Delivery Gaps


To identify the 10 constituencies with the lowest JJM functional tap connection coverage and examine geographic patterns in scheme delivery across Meghalaya.

Steps I followed:
1. Opened 'Sample meghalaya constituency data' in Excel.
2. Used 'Data' → 'Sort' to sort the entire dataset by 'JJM Functional Tap Connection' from 'Smallest to Largest'.
3. Selected the first 10 rows after sorting as the constituencies with lowest JJM coverage.
4. Counted constituencies by region to check for geographic concentration.
5. Created a clustered bar chart of 'JJM Coverage %' for the bottom 10 constituencies.

Findings:
The 10 constituencies with lowest JJM coverage are:

| Rank | Constituency | Region | JJM Coverage % |
| --- | --- | --- | --- |
| 1 | Kharkutta | Garo Hills | 24.1 |
| 2 | Khliehriat | Jaintia Hills | 24.1 |
| 3 | Sohiong | Khasi Hills | 26.6 |
| 4 | Mendipathar | Garo Hills | 27.1 |
| 5 | Selsella | Garo Hills | 27.4 |
| 6 | Mawphlang | Khasi Hills | 27.4 |
| 7 | Songsak | Garo Hills | 27.6 |
| 8 | Williamnagar | Garo Hills | 28.2 |
| 9 | Ampati | Garo Hills | 28.4 |
| 10 | Umsning | Khasi Hills | 28.4 |

Regional count: 6 Garo Hills, 3 Khasi Hills, 1 Jaintia Hills. JJM coverage in these areas ranges from 24.1% to 28.4%, compared to the state average of 57.3%.

Data Analysis:
JJM delivery gaps are heavily concentrated in Garo Hills, which has 6 of the 10 worst-performing constituencies. Kharkutta and Mendipathar show less than 28% household coverage, meaning 3 in 4 homes lack functional tap connections. This reflects Garo Hills’ challenges of hilly terrain, sparse road networks, and weaker administrative reach. Khasi Hills constituencies like Sohiong and Mawphlang also appear, indicating that high rainfall damages pipelines and tanks, causing service failures even in developed areas. Khliehriat in Jaintia Hills suggests mining zones face water contamination and infrastructure neglect. The pattern shows geography and infrastructure access drive scheme failure more than poverty alone. Policy must prioritize last-mile connectivity and climate-resilient pipelines in Garo Hills, plus better maintenance funding for Khasi Hills monsoon damage. Without region-specific interventions, JJM will not achieve universal coverage in Meghalaya. 


### Section 2 Q3: Fund Utilisation


To identify the five constituencies with the lowest Constituency Development Fund utilisation and analyse associated patterns.

The dataset was sorted by 'constituency fund untilized' in ascending order. The bottom five constituencies were extracted and compared with `BPL_Households' using a clustered column chart.

Findings:

The lowest fund utilisation was observed in Khliehriat (44.2%), Mendipathar (45.8%), Songsak (47.1%), Selsella (48.3%), and Williamnagar (49.2%). Four are in Garo Hills. All five exhibit high BPL rates (58.3%–64.8%) and low JJM coverage (24.1%–28.2%), indicating poverty and infrastructure deficits.

Hypothesis:

Underutilisation likely stems from:

1) Geographic remoteness raising project costs
3) Limited administrative capacity in poor constituencies
5) Delays in clearances for land and forests and,
6)  A cyclical poverty-trap where weak governance leads to unspent funds and continued underdevelopment.
