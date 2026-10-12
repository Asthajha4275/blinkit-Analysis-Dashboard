# Blinkit Grocery Sales Analysis

An analysis of Blinkit grocery sales, customer ratings and outlet performance, built from a business requirement document (BRD) of four KPIs and seven charts. The workbook summarises the data with PivotTables and brings everything together in a dashboard.

**Tools:** Microsoft Excel (data cleaning, PivotTables, charts, dashboard)

---

## 1. Business Requirement

To analyse Blinkit's **sales performance, customer satisfaction and inventory distribution**, identifying insights and optimisation opportunities using KPIs and visualisations.

### KPIs
| KPI | Definition |
|---|---|
| Total Sales | Overall revenue from all items sold |
| Average Sales | Average revenue per sale |
| Number of Items | Total count of items sold |
| Average Rating | Average customer rating of items sold |

### Charts requested
| # | Chart | Objective | Chart type |
|---|---|---|---|
| 1 | Total Sales by Fat Content | Impact of fat content on sales | Donut |
| 2 | Total Sales by Item Type | Which item types perform best | Bar |
| 3 | Fat Content by Outlet (Total Sales) | Sales by outlet, split by fat content | Stacked column |
| 4 | Total Sales by Establishment | How outlet age affects sales | Line |
| 5 | Sales by Outlet Size | Relationship between outlet size and sales | Donut / Pie |
| 6 | Sales by Outlet Location | Geographic distribution of sales | Funnel / Map |
| 7 | All Metrics by Outlet Type | All four KPIs side by side | Matrix card |

---

## 2. Dataset

| Item | Detail |
|---|---|
| File | `BlinkIT Grocery Data Excel.xlsx` (sheet: `BlinkIT Grocery Data`) |
| Size | 8,523 item records × 13 columns |
| Columns | Item Identifier, Item Fat Content, Item Type, Item Weight, Item Visibility, Outlet Identifier, Outlet Establishment Year, Outlet Size, Outlet Location Type, Outlet Type, Total Sales, Rating |
| Outlets | 10 outlets across 3 location tiers and 4 outlet types |

**Data quality notes:** Fat content was recorded inconsistently ("Low Fat", "low fat", "Regular") and had to be standardised. About 1,460 records have no Item Weight; this field is not used in the KPIs.

---

## 3. Project Steps

### Step 1 – Understand the requirement
Read the BRD and listed the four KPIs and seven charts to be delivered.

### Step 2 – Load and clean the data
- Imported the Blinkit data into Excel.
- Standardised the Item Fat Content labels so that "Low Fat" and "low fat" count as one category.
- Checked for duplicates (none) and for missing values (only Item Weight).

### Step 3 – Calculate the KPIs
Built the KPI table with PivotTables / formulas:

| Total Sales | Average Sales | Number of Items | Average Rating |
|---|---|---|---|
| 1,201,681 | 140.99 | 8,523 | 3.97 |

### Step 4 – Build the PivotTables
One PivotTable per chart on the `Pivot table` sheet: sales by fat content, by item type, by outlet tier and fat content, by establishment year, by outlet size, by outlet location, and sales / average sales / item count / rating by outlet type.

### Step 5 – Create the charts
Turned each PivotTable into the chart type requested in the BRD (donut, bar, stacked column, line, pie, map/funnel, matrix card).

### Step 6 – Build the dashboard
Placed the KPI cards and all charts on the `DASHBOARD` sheet for a one-page view of Blinkit's performance.

### Step 7 – Draw insights
See the next section.

---

## 4. Key Insights

- **Total sales are about 1.2M** from 8,523 items, at an average of about 141 per sale, with an average rating of 3.97.
- **Low Fat items drive ~65% of sales** (776K) vs. ~35% for Regular (425K).
- **Top item types:** Fruits and Vegetables (178K) and Snack Foods (175K) lead, followed by Household and Frozen Foods. Seafood (9K) and Breakfast (16K) are the smallest.
- **Outlet location:** Tier 3 contributes the most sales (~39%, 472K), then Tier 2 (393K) and Tier 1 (336K). Low Fat leads Regular in every tier.
- **Outlet size:** Medium outlets bring in ~42% of sales, Small ~37%, High ~21%.
- **Outlet type:** Supermarket Type1 generates ~66% of sales (788K), mainly because it sells far more items (5,577) than the others. Average sales per item are almost identical across outlet types (about 140–142).
- **Establishment year:** Outlets established in 2018 have the highest sales (205K), while the 2011 outlet is lowest (78K).

---

## 5. Recommendations

1. **Stock more Low Fat, fruit and vegetable, and snack items**, which are the biggest sales drivers.
2. **Invest in Tier 3 and Tier 2 locations** and in Medium-sized outlets, where sales are highest.
3. **Grow Supermarket Type1**: sales per item are similar across outlet types, so more items sold means more revenue.
4. **Review the weakest outlets and low-selling categories** (such as Seafood and Breakfast) for range or promotion changes.
5. **Work on ratings**, which average below 4, by improving product quality and availability.

---

## 6. Repository Structure

```
├── BlinkIT Grocery Data Excel.xlsx   # Data, PivotTables, charts, dashboard
├── Blinkit_Analysis.pdf              # Business requirement document
└── README.md
```

## 7. Skills Demonstrated

Requirement analysis · Data cleaning · KPI design · PivotTables · Data visualisation · Dashboarding · Business insight generation

---
## Architecture Diagram
![Blinkit Architecture](diagram%20(3).png)


**Author:** Astha Kumari Jha
**GitHub:** [github.com/Asthajha4275](https://github.com/Asthajha4275)# blinkit-Analysis-Dashboard

