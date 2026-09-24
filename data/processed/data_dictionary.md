# Banking Dataset Data Dictionary

## 1. Numerical Columns

Numerical columns:
- age
- balance
- day
- duration
- campaign
- pdays
- previous

| Column | Summary / Observation |
|--------|----------------------|
| age | Age distribution is healthy and does not contain negative values. |
| balance | Balance is highly skewed. Minimum value is -3313, with 366 negative values and 733 rows at or below 0. This may need further investigation. |
| day | Day values have a reasonable spread from 0 to 31, with no visible issue. |
| duration | Last contact duration in seconds. This feature appears to strongly affect the outcome. |
| campaign | Number of calls made to the client during the current campaign. The distribution is right-skewed. |
| pdays | Number of days since the client was contacted in a previous campaign. A value of -1 means the client was not contacted before. |
| previous | Number of calls made before the current campaign. Data is unevenly distributed. |

### Balance Summary
| Statistic | Value |
|-----------|-------|
| count | 4521.000000 |
| mean | 1422.657819 |
| std | 3009.638142 |
| min | -3313.000000 |
| 25% | 69.000000 |
| 50% | 444.000000 |
| 75% | 1480.000000 |
| max | 71188.000000 |

### Duration Summary
| Statistic | Value |
|-----------|-------|
| count | 4521.000000 |
| mean | 263.961292 |
| std | 259.856633 |
| min | 4.000000 |
| 25% | 104.000000 |
| 50% | 185.000000 |
| 75% | 329.000000 |
| max | 3025.000000 |

## 2. Categorical Columns

Categorical columns:
- job
- marital
- education
- default
- housing
- loan
- contact
- month
- poutcome
- y

| Column | Unique Values |
|--------|---------------|
| job | unemployed, services, management, blue-collar, self-employed, technician, entrepreneur, admin., student, housemaid, retired, unknown |
| marital | married, single, divorced |
| education | primary, secondary, tertiary, unknown |
| default | no, yes |
| housing | no, yes |
| loan | no, yes |
| contact | cellular, unknown, telephone |
| month | jan, feb, mar, apr, may, jun, jul, aug, sep, oct, nov, dec |
| poutcome | success, failure, other, unknown |
| y | no, yes |

### Unique Count Summary
| Column | Unique Count |
|--------|--------------|
| job | 12 |
| marital | 3 |
| education | 4 |
| default | 2 |
| housing | 2 |
| loan | 2 |
| contact | 3 |
| month | 12 |
| poutcome | 4 |
| y | 2 |

## 3. Key Observations

- Age is well distributed and contains no negative values.
- Balance has a large number of zero or negative values, which may need deeper investigation.
- Duration is likely one of the strongest predictors of the target variable.
- Some customers were still uncontacted, and their previous outcomes are unknown.
- Campaign-related features are skewed and may require transformation during modeling.

