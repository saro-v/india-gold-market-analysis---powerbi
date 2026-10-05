# KPIs and Power BI Measures

The final report uses a small set of DAX calculations.

## Page 1

### Gold 22K Rate

```DAX
Gold 22K Rate =
CALCULATE(
    MAX(Daily_Bullion_Rates[Rate]),
    Daily_Bullion_Rates[Metal] = "Gold",
    Daily_Bullion_Rates[Purity] = 916,
    Daily_Bullion_Rates[Session] = "PM"
)
```

### Silver 999 Rate

```DAX
Silver 999 Rate =
CALCULATE(
    MAX(Daily_Bullion_Rates[Rate]),
    Daily_Bullion_Rates[Metal] = "Silver",
    Daily_Bullion_Rates[Purity] = 999,
    Daily_Bullion_Rates[Session] = "PM"
)
```

### Gold Karat

```DAX
Gold Karat =
SWITCH(
    Daily_Bullion_Rates[Purity],
    999, "24K",
    916, "22K",
    750, "18K",
    585, "14K",
    BLANK()
)
```

## Page 2

### Total Gold Consumption

```DAX
Total Gold Consumption =
SUM(
    State_Gold_Consumption[EstimatedGoldConsumption_tonnes]
)
```

### Top Consuming State

The report ranks states by the sum of the estimated consumption field and returns the highest state.

### Leading Region Share

The report ranks regions by total estimated consumption and returns the leading region together with its share of the total.

## Important

The DAX measures describe the dashboard calculations. They do not change the underlying source status of the data. In particular, the state-level figures remain analytical estimates.
