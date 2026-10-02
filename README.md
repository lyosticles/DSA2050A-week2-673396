# Customer, Order and Region Sales Analysis

### John Lyomoki - 673396

## Objective

This project analyzes customer and order data to understand how sales vary across customer segments and regions. It cleans and validates the source tables, joins orders to customers and regions while guarding against duplicate keys and unmatched records, and reconciles totals after each join. The result is a set of reliable segment and region KPIs that management can use to see where revenue comes from.

## Key Findings

1. **Data quality issues affected the join.** The customers table contained a duplicate CustomerID C004, which would have inflated order counts and totals through copies if left in place. At least one order had no matching customer, so it appeared with no Segment or Region and could not be attributed (9,900 in sales).

2. **Corporate is the highest-value segment.** Corporate generated the most sales 46,800 from only 4 orders, averaging 11,700 per order.

3. **Nairobi leads in total sales, but this does not prove it performs best.** Nairobi recorded 39,800 from 7 orders, yet its average order value (about 5,686) is the lowest of the named regions, but the sample was very small to be conclusive on weather it was the best performing region.
