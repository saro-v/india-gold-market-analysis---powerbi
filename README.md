# India Gold Market Analysis | Power BI

A Power BI academic project on gold prices, gold consumption and demand in India, with supporting silver price trends.

## About the project

This report was built as a compact two-page dashboard.

**Page 1 — Gold & Silver Market Pulse**  
Looks at 22K gold, 999 silver, price movement and gold rates by purity.

**Page 2 — India Gold Consumption & Demand**  
Looks at estimated state-wise consumption, regional demand, demand segments and selected jeweller rates.

The main idea is simple: start with the market price, then move to where gold demand is concentrated across India.

## What is included

- Final Power BI report (`.pbix`)
- Four core CSV data tables
- Final Excel workbook
- Two dashboard images
- Project documentation and presentation notes

## Data note

The dashboard uses the latest published observations included in the project dataset; it is not a live market feed.

The state-wise gold-consumption values are **analytical estimates**, not official state-level statistics. They were prepared using published regional demand shares and state allocation weights. This limitation is kept visible in the project documentation.

## Main data sources

- Indian Bullion and Jewellers Association (IBJA) — bullion rates
- Economic Times — selected 22K jeweller retail-rate observations
- World Gold Council — India gold-demand figures and regional demand information

More detail is available in [`docs/sources-and-limitations.md`](docs/sources-and-limitations.md).

## Repository structure

```text
India_Gold_Market_Analysis/
├── README.md
├── index.html
├── assets/
│   ├── dashboard-page-1.png
│   └── dashboard-page-2.png
├── data/
│   ├── Daily_Bullion_Rates.csv
│   ├── Jeweller_Retail_Rates.csv
│   ├── India_Gold_Demand.csv
│   ├── State_Gold_Consumption.csv
│   └── Gold_Silver_PowerBI_Final_Compact_Dataset.xlsx
├── docs/
│   ├── project-overview.md
│   ├── data-dictionary.md
│   ├── methodology.md
│   ├── kpi-and-measures.md
│   ├── dashboard-guide.md
│   ├── sources-and-limitations.md
│   ├── presentation-notes.md
│   └── github-upload-guide.md
└── powerbi/
    └── India Gold Market Analysis.pbix
```

## How to use the project

Open the `.pbix` file in Power BI Desktop to view or edit the report. The CSV files and Excel workbook are included so the data structure can be reviewed separately.

For the GitHub website, open `index.html` through GitHub Pages.

## Academic note

This project is intended for academic analysis and presentation. It is not investment advice.
