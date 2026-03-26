# E-Commerce Profitability Analysis
**True profit analysis across product categories, sales channels, and marketing spend**

---

## What This Project Does

Top-line revenue looked healthy at **$2.38M** — but that number was masking a more complicated story underneath. This analysis peels back gross revenue to find where the business is *actually* making money, and where it is quietly losing it.

Using 12,000 orders across a full fiscal year, the analysis connects three data sources — order transactions, product costs, and marketing spend — to produce a single, honest picture of profitability after accounting for shipping, returns, platform fees, and advertising costs.

---

## The Bottom Line (Executive Summary)

| Metric | Value |
|---|---|
| Gross Revenue | $2,384,561 |
| Revenue Lost to Returns | **$236,896** (9.9% of gross) |
| Net Profit | **$565,692** |
| Overall Profit Margin | **26.3%** |
| Total Marketing Spend | $625,912 |
| Blended Marketing ROAS | 22.4× |

The business is profitable — but two categories and one marketing platform are quietly dragging the whole operation down.

---

## Key Finding 1 — Not All Products Are Equal

**Beauty and Home & Garden are carrying the business. Electronics is the problem.**

| Category | Profit Margin | Return Rate | Avg Profit / Order |
|---|---|---|---|
| Beauty | **50.5%** | 8.6% | $40.97 |
| Home & Garden | **41.1%** | 9.5% | $132.20 |
| Sports | 39.1% | 9.0% | $77.04 |
| Apparel | 34.4% | 21.6% | $31.10 |
| Food & Grocery | 21.1% | 2.4% | $7.80 |
| Books & Media | 18.6% | 3.8% | $6.39 |
| **Electronics** | **7.7%** | 11.2% | $37.59 |

**Why Beauty wins:** High markup (products sell at 2.5–4.5× their cost) combined with a low return rate means almost every sale is clean profit.

**Why Electronics struggles:** Product cost alone consumes ~62 cents of every $1 earned. Add an 11.2% return rate — where customers are returning expensive items — and margins collapse. Electronics is generating volume but not value.

> **Apparel return rate of 21.6% is a red flag.** One in five Apparel orders is returned, costing an estimated $75,000+ in refunds over the year — the single largest return-driven revenue loss in the business.

---

## Key Finding 2 — Where You Sell Matters as Much as What You Sell

**Selling on Marketplace costs the business $27.59 per order compared to selling on the Website.**

| Channel | Avg Profit / Order | Profit Margin | Platform Fee |
|---|---|---|---|
| Website | **$56.59** | 31.2% | 0% |
| Mobile App | $50.42 | 28.9% | 2% |
| Social Commerce | $43.57 | 24.1% | 6% |
| **Marketplace** | **$29.00** | 16.2% | **12%** |

Marketplace charges a 12% fee on every transaction. That single line item is the primary reason Marketplace profit per order is nearly half that of the Website — before returns are even considered. With roughly 26% of all orders coming through Marketplace, the cumulative profit cost is substantial.

---

## Key Finding 3 — One Marketing Platform Is Burning Money

**Influencer marketing spent $97,327 and delivered the worst return of any channel.**

| Platform | Annual Spend | ROAS | Cost Per Acquisition |
|---|---|---|---|
| Email Marketing | $20,789 | **352×** | **$0.77** |
| Meta / Facebook | $153,842 | 15.3× | $19.21 |
| Google Ads | $169,024 | 13.9× | $24.24 |
| TikTok Ads | $83,324 | 10.5× | $17.27 |
| YouTube Ads | $69,961 | 8.2× | $36.71 |
| Pinterest Ads | $31,644 | 6.0× | $29.33 |
| **Influencer** | **$97,328** | **3.5×** | **$60.30** |

*ROAS = Revenue generated per $1 spent. Higher is better.*

Email Marketing is the standout — at $0.77 cost per customer acquired, it is 78 times more efficient than Influencer. Every month of Influencer spend in 2024 fell below a 4× return. Pinterest Ads also underperformed, with two months dipping below 3×.

---

## Three Recommendations

### 1. Cut Influencer Budget — Reallocate to Email and Meta
Influencer marketing is the lowest-returning channel in the portfolio. Eliminating it saves **$97,328 per year**. Redirecting half to Email (owned channel, near-zero marginal cost) and half to Meta covers the 20% budget reduction target entirely, with minimal revenue impact. The revenue Influencer was attributed with can be recaptured more efficiently elsewhere.

**Budget cut target achieved: $125,182 saved (20% of total spend)**
Specific months to cut first: Influencer — October, September, January, June, November (lowest ROAS months, all below 3.5×).

### 2. Fix the Electronics Margin Problem
Electronics needs either lower costs or higher prices. Three levers available:
- **Renegotiate supplier pricing** — a 10–15% unit cost reduction would add an estimated $30–40K to annual profit
- **Tighten the return policy** — reducing the 11.2% return rate to the 8–9% range seen in other categories meaningfully reduces costly refunds
- **Reprice Accessories** — this sub-category has pricing headroom that is currently untapped

### 3. Migrate Marketplace Customers to Direct Channels
Every Marketplace customer converted to a Website customer is worth **$27.59 more in profit** per order. With 12% of revenue going directly to the platform as fees, reducing Marketplace dependency is one of the highest-leverage moves available. Suggested tactics: include website discount codes in Marketplace packaging, invest in direct SEO/SEM, and introduce a loyalty programme exclusive to direct-channel buyers.

**Combined impact of all three recommendations: estimated $195–250K additional annual profit, improving overall margin from 26.3% toward 32–35%.**

---

## Project Structure

```
ecommerce-profitability-analysis/
│
├── data/
│   ├── products.csv          # 126 products across 7 categories
│   ├── orders.csv            # 12,000 orders (FY 2024)
│   └── marketing_spend.csv   # Monthly spend by platform (7 platforms × 12 months)
│
├── analysis/
│   └── profitability_analysis.py   # Full Python analysis (pandas)
│
├── dashboard/
│   └── dashboard.html        # Interactive profitability dashboard
│
└── README.md
```

---

## How to Run

```bash
# Install dependencies
pip install pandas numpy

# Generate datasets
python analysis/generate_data.py

# Run full analysis
python analysis/profitability_analysis.py
```

**Requirements:** Python 3.8+, pandas, numpy

---

## Tools Used

- **Python / pandas** — data loading, aggregation, profitability calculations
- **Chart.js** — interactive dashboard visualisations
- **Data sources:** Synthetic datasets modelled on realistic South African e-commerce market dynamics (pricing, categories, channels)

---

## Skills Demonstrated

- Order-level profitability analysis (connecting revenue, costs, returns, and fees)
- Marketing ROI analysis (ROAS, CPA, spend efficiency)
- Channel and category benchmarking
- Budget optimisation with data-backed recommendations
- Executive reporting — translating data findings into business decisions

---

*Analysis period: January – December 2024 | Orders analysed: 12,000 | Data verified: 100% cost reconciliation passed*
