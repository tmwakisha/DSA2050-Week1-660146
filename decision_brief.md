# Decision brief: Retail product pilot

**Business problem.** Retail leadership needs to prioritize a bounded sales test from a one-quarter transaction extract, without treating sales revenue as profit.

**Stakeholder.** Retail leadership and store operations.

**Decision.** Select a product for a small, controlled next-quarter merchandising/availability pilot. The analysis suggests testing Office Chairs, but does not justify broad inventory expansion.

**Unit of analysis.** One recorded transaction/order (`OrderID`); the extract has 300 rows and 11 columns covering 1 January–31 March 2026.

**Three KPIs.** Total revenue = sum of `Revenue_KES` = **KES 3,206,450**; transactions = distinct `OrderID` = **300**; average transaction value = total revenue / transactions = **KES 10,688.17**. The last two are counts and sales-value metrics, not profit or customer lifetime value.

**Initial findings.** Office Chairs lead product revenue at **KES 594,500 (18.5%)**, from 12 orders; Perfume follows at KES 313,500. Monthly revenue is KES 928,900 in January, KES 909,900 in February, and KES 1,367,650 in March. March is higher, but the short period provides no basis to infer a durable trend or its cause.

**Recommendation and limitation.** Test chair merchandising/availability for one month against a comparable holdout; judge on incremental gross profit and monitor stock-outs, returns, discounts, and cannibalization. The dataset has no cost, inventory, discount, return, promotion, or causal-control fields. It cannot establish profitability, constrained demand, or future growth.

**Workflow.** See `week1_analysis.ipynb` for the load/inspection, data-quality and descriptive-statistics checks, KPI calculations, two labelled plots with interpretations, and conclusion. Run it from the project root after installing `requirements.txt`.
