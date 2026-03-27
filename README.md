# E-Commerce Profitability Analysis
**True profit analysis across product categories, sales channels, and marketing spend**

---

## What This Project Does

Top-line revenue looked healthy at **$278.0K** — but that number was masking a more complicated story underneath. This analysis peels back gross revenue to find where the business is *actually* making money, and where it is quietly losing it.

Using 2000 orders across a full fiscal year, the analysis connects three data sources — order transactions, product costs, and marketing spend — to produce a single, honest picture of profitability after accounting for shipping, returns, platform fees, and advertising costs.

---

## The Bottom Line (Executive Summary)

| Metric | Value |
|---|---|
| Gross Revenue | **$277,969.13** |
| Revenue Lost to Returns | **$20,582.45** (7.4% of gross) |
| Net Profit | **$236,318.37** |
| Overall Profit Margin | **23.8%** |
| Total Marketing Spend | $503,506.14 |
| Blended Marketing ROAS | 16.2x |

---

## Key Finding 1 — Not All Products Are Equal

**Electronics and Toys are carrying the business. Books is the weakest link.**

 |primary_category | profit_margin | return_rate | avg_profit_per_order
 |---|---|---|---| 
 | Electronics | 31.13%    | 8.61% | $52.34
 | Toys | 26.15% | 7% | $34.19
 | Home & Kitchen | 25.37% | 6% | $33.44
 | Food & Beverage | 24.76% |5.67% |$30.74
 | Sports | 23.5% | 7.19% | $26.02
 | Clothing | 19.97% | 8.19% | $21.41
 | Beauty | 17.39% | 5.59% | $15.49
 | Books | 11.93% | 8.37% | $9.41
---

**Electronics** earns $52.34 profit per order — 5.6× more than Books at $9.41. The 19.2-point margin gap between the best and worst category is the single biggest profitability lever in the business.

> **As much as Electronics drives revenue, its return rate of 8.61% is a red flag.**
> Costing an estimated $4000+ in refunds over the year.

---

## Key Finding 2 — Where You Sell Matters as Much as What You Sell

**Selling on Marketplace costs the business approx. $21 per order compared to selling on the Mobile App.**

|channel | profit_margin | total_platform_fees | avg_profit_per_order
|---|---|---|---|
| Marketplace | 13.03%| 16.06% | $15.39
| Mobile App | 29.76% | 0.0% | $36.32
| Social Commerce | 15.37% | 8.87%| $17.11|
| Website| 27.015% | 0.0%| $31.59

**Marketplace's 16% platform fee coststhe business approx. $21 in profit per order compared to the Mobile App, before returns are considered. With 20.95% of orders coming through Marketplace, this fee drag compounfs significantly across the year.**

---

## Key Finding 3 — One Marketing Platform Is Burning Money

**Email Marketing spent $24,461.37 and delivered the worst return of any channel.**

|platform| annual spend | roas| avg_cpa
|---|---|---|---|
| Email Marketing | $24,461.37 | 4.81x | $26.01
| Facebook Ads| $106,451.93 | 11.45x | $8.38
| Google Ads| $152,546.48 | 14.38x | $6.48
| Influencer | $97,663.12 | 22.70x | $4.79
| Instagram Ads | $65,154.02 | 15.73x | $5.55
| TikTok Ads | $57,229.22 | 24.02x | $3.93
        
*ROAS = Revenue generated per $1 spent. Higher is better.*

**TikTok Ads Marketing is the standout at $3.93 cost per customer acquired, it is 7 times more efficient than Email Marketing.**

---

## Three Recommendations

### 1. Cut Email Marketing Budget — Reallocate to TikTok Ads and Influencers
Email marketing is the lowest-returning channel in the portfolio. Eliminating it saves **$24,461.37 per year**. Redirecting half to TikTok Ads and half to Influencers covers the 20% budget reduction target entirely, with minimal revenue impact.

**Budget cut target achieved: $100,701.228 saved (20% of total spend)**
Specific months to cut first: Email Marketing — December, October, July, June, November (lowest ROAS months, all below 3.5×).

### 2. Fix the Bookd Margin Problem
Books needs either lower costs or higher prices.
- **Renegotiate supplier pricing** — a unit cost reduction would add more cash to annual profit
- **Tighten the return policy** — reducing the 8.37% return rate to the 3–5% range will meaningfully reduce costly refunds

### 3. Migrate Marketplace Customers to Direct Channels
Every Marketplace customer converted to a Mobile App customer is worth **$20.93 more in profit** per order. With 16% of revenue going directly to the platform as fees, reducing Marketplace dependency is one of the highest-leverage moves available. 

Suggested tactics: include Website discount codes in Marketplace packaging, and introduce a loyalty programme exclusive to direct-channel buyers.

---

## Tools Used

- **Python / pandas** — data loading, aggregation, profitability calculations
- **Plotly** — dashboard visualisations
- **Data sources:** Datasets on BrightCart e-commerce market. BrightCart is an online retailer selling products across 8 categories through their website, mobile app, third-party marketplaces, and social commerce. 
---

## Skills Demonstrated

- Order-level profitability analysis (connecting revenue, costs, returns, and fees)
- Marketing ROI analysis (ROAS, CPA, spend efficiency)
- Channel and category benchmarking
- Budget optimisation with data-backed recommendations
- Executive reporting — translating data findings into business decisions

---
