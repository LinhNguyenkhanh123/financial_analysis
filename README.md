# Financial Analysis Dashboard

## 1. Project Overview

This Power BI report evaluates the company's financial performance across **revenue, expenses and profit**, broken down by **Business Line** and over time. It aims to answer: where does the company make money, where do costs go, which business lines perform best, and what actions should be prioritized?

| Item | Description |
|---|---|
| **Tool** | Power BI Desktop (custom visual: Dumbbell Chart) |
| **Data model** | Fact table `revenue_expense` (Amount, Date, Business Line) joined with `dimDate` and `dimRevenue/expense_group` (revenue/expense groups, expense subgroups) |
| **Key measures** | Total Revenue, Net Revenue, Gross Profit, EBIT, Net Profit, Net Profit Margin, Operating Margin, COGS, Operating Expenses, Total Expenses, Expense/Revenue, Efficiency Ratio, % Revenue Contribution, Break-even Point (BEP), plus growth measures |
| **Business lines analyzed** | Sportswear, Sports Equipment, Nutrition & Food Supplements, Consulting & Professional Services |

### Report Structure

| Page | Content | Key question |
|---|---|---|
| **Executive Summary** | Headline KPIs (Revenue, Expenses, Net Profit, Net Profit Margin, Efficiency Ratio) with yearly trends, waterfall, donut and decomposition tree | *How does Revenue become Profit? Where do Revenue and Expenses come from?* |
| **Revenue Analysis** | Revenue-to-Net-Profit funnel, growth vs. margin scatter, margin by business line combo chart, action matrix (Expand / Invest / Review / Optimize cost) | *Which business lines are both growing and profitable?* |
| **Expense Analysis** | Cost structure (COGS, Opex, Interest & Tax), cost growth vs. revenue growth, cost efficiency scatter | *What drives total expenses? Are costs outpacing revenue?* |
| **Recommendations** | Overall, revenue/profitability and cost optimization recommendations, plus break-even gauges | *What should we do next?* |
| **Tooltip 1–3** | Hidden tooltip pages: COGS/Opex, revenue by business line, expenses by subgroup | Detail on hover |

**Interactivity:** Business Line and Month slicers, parameter switches, page navigator and custom tooltips.

---

## 2. Main Findings

1. **The company is still profitable, but growth is slowing.** Revenue and profit growth rates have declined significantly, and only started to recover from **December**.
2. **Revenue depends on the core business.** **Sales accounts for 78.46%** of total revenue.
3. **Profitability varies widely across business lines:**

| Business Line | Revenue | Net Profit Margin | Notes |
|---|---|---|---|
| **Sportswear** | ~$5.11M | **20.26%** (highest) | Revenue **down 7.50%**; high margin may partly reflect higher prices, which could push price-sensitive customers to competitors |
| **Sports Equipment** | – | 7.31% | Lower margin than Sportswear |
| **Nutrition & Food Supplements** | ~$1.53M | **-66.92%** (net loss ~$768,470) | Revenue too low to cover fixed costs, especially Equipment; possible extra costs from product disposal or heavy discounting near expiry |
| **Consulting & Professional Services** | ~$2.82M | **-370.21%** | Heavy reliance on senior staff with high labor costs |

4. **Cost pressure is shifting from direct costs to operating costs:**
   - COGS **decreased ~16.44%**, while Operating Expenses **increased ~12.09%**.
   - Interest & Tax expenses also grew relatively quickly.
5. **Labor is the largest cost category:** **$4.49M, or 33.91% of total costs**, yet it contributes only **27.07% of revenue**, suggesting labor productivity is not keeping pace with cost.

---

## 3. Main Recommendations

### Overall
- **Prioritize Sportswear and Sports Equipment**, while reviewing low-margin product groups before further expansion.
- **Regularly review high-growth expense categories** to keep the overall cost structure under control.

### Revenue & Profitability
1. **Recover Sportswear growth while protecting its margin.** Use cross-selling programs with other product groups to rebuild sales volume without discounting.
2. **Nutrition & Food Supplements: set a break-even deadline.** If the target is not met, test an **outsourcing model** to eliminate Equipment and warehouse costs.
3. **Consulting & Professional Services: restructure.** Raise service prices and/or restructure the team, keeping only employees with high utilization rates.

### Cost Optimization
1. **Improve labor cost efficiency.** Move staff from loss-making areas (Consulting, Nutrition) to support Sportswear, and consider shifting part of fixed salaries to performance-based pay.
2. **Control Operating Expense growth.** Renegotiate outsourcing, office supply and third-party service contracts, and require departments to justify Opex budgets and major expenses.
