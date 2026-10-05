# Data Dictionary

The Power BI report uses four core tables.

## 1. Daily_Bullion_Rates

| Column | Meaning | Unit |
|---|---|---|
| Date | Observation date | Date |
| Metal | Gold or Silver | — |
| Purity | Purity code | — |
| Session | AM or PM | — |
| Rate | Published bullion rate | See Unit |
| Unit | Quoted rate unit | — |

Gold purity codes used in the report include 999, 916, 750 and 585. These are displayed as 24K, 22K, 18K and 14K.

## 2. Jeweller_Retail_Rates

| Column | Meaning | Unit |
|---|---|---|
| Date | Observation date | Date |
| Jeweller | Jeweller name | — |
| City | City of observation | — |
| State | State/UT of the city | — |
| Gold22K_INR_per_g | Observed 22K retail rate | INR/g |

These rates are for comparison. They are not a single official retail rate for India.

## 3. India_Gold_Demand

| Column | Meaning | Unit |
|---|---|---|
| Quarter | Reporting quarter | — |
| Segment | Jewellery, Bar & Coin or Gold ETF | — |
| DemandTonnes | India gold demand | tonnes |
| DemandValue_INRbn | Demand value | INR billion |

## 4. State_Gold_Consumption

| Column | Meaning | Unit |
|---|---|---|
| Quarter | Quarter used for the estimate | — |
| State | State/UT | — |
| Region | North, South, East or West | — |
| EstimatedGoldConsumption_tonnes | Analytical state estimate | tonnes |
| Basis | Basis of the estimate | — |

### Note

The state table is **derived data**. It should not be described as official state-wise consumption statistics.
