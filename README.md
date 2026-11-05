# DSA2050 Week 1 — Retail Analysis

**Student name:** Samara Mwalisha  
**Student ID:** 660146

## Project objective
Use the supplied retail transactions to describe sales patterns and frame one cautious, evidence-based decision a retailer could test. The analysis is descriptive and does not estimate profit or causal impact.

## Three KPIs
1. Total revenue = sum of `Revenue_KES` (KES 3,206,450).
2. Number of transactions = distinct `OrderID` (300).
3. Average transaction value = total revenue / distinct transactions (KES 10,688.17).

## Two key findings
- Office Chairs are the top product by recorded revenue (KES 594,500, 18.5%), but this comes from 12 orders.
- March revenue (KES 1,367,650) is higher than February (KES 909,900); this three-month extract cannot establish the cause or persistence.

## Project structure
- `retail.csv` — supplied input data
- `week1_analysis.ipynb` — runnable notebook with required inspection, diagnostics, three KPIs, and two interpreted plots
- `decision_brief.md` — concise decision brief
- `requirements.txt` — pinned dependencies

## Run
From this directory:

```bash
pip install -r requirements.txt
jupyter notebook week1_analysis.ipynb
```

The notebook reads `retail.csv` using a relative path. Restart the kernel and run all cells from top to bottom.
