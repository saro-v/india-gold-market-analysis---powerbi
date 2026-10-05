# Methodology

## Price analysis

The bullion table contains daily gold and silver observations. The main headline rates use the **PM session** for consistency.

Gold purity is shown in common karat terms:

- 999 → 24K
- 916 → 22K
- 750 → 18K
- 585 → 14K

The dashboard uses the wording **Latest Published Data** rather than real-time data.

## Jeweller rates

The retail table contains observed 22K rates by jeweller and city. These values are used as a comparison point, not as a universal retail price.

## India gold demand

Quarterly India demand is kept in a separate table and is shown by segment:

- Jewellery
- Bar & Coin
- Gold ETF

## State-wise consumption estimate

A current official state-by-state consumption series was not available in the required form. The project therefore uses a transparent analytical allocation:

1. Start with the published India jewellery-demand total for the relevant quarter.
2. Apply the published regional demand shares.
3. Allocate the regional amount across selected states using predefined state weights.
4. Check that the state allocations reconcile with the regional totals.
5. Keep the result labelled as an estimate.

The state table includes a `Basis` field for this reason.

## Quality checks

The final dataset was checked for consistent column names, dates, state/region labels, units, purity codes, non-negative values and reconciliation of the state allocation.

## Interpretation

The dashboard is an academic analytical view. It is not a live trading system and is not investment advice.
