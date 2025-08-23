# Marketing Mix Modeling: Reported vs. Modeled Revenue

## 📌 Overview
This project explores why **reported revenue from advertising platforms** (e.g., Facebook Ads, Google Ads, Pinterest) often differs from **modeled revenue derived through marketing mix modeling (MMM)**.  

I designed this analysis to uncover:
- Why reported revenue tends to be **inflated** relative to modeled revenue.  
- How modeling incremental lift (rather than influenced revenue) provides more accurate insights.  
- What this means for **budget allocation, ROI measurement, and marketing strategy**.

The project compares data across **development (dev)** and **production (prod)** environments, showing how marketing data evolves from a controlled test setting into real-world complexity.

---

## 🎯 Motivation
Ad platforms have a vested interest in reporting inflated numbers — they want advertisers to see their channel as indispensable. However, business decisions require more **causal, conservative, and actionable metrics**.  

By using MMM, I shift the perspective from **influence** to **incrementality**:
- **Reported Revenue** = All influenced sales claimed by a channel.  
- **Modeled Revenue** = Only the causal lift attributable to spend.  

This reframing enables sharper, evidence-based decisions on where the **next marketing dollar** should go.

---

## 📊 Key Analyses & Insights

### 1. Reported Revenue (Dev vs. Prod)
- **Dev**: Cleaner, aggregated data; smooth and stable trends.  
- **Prod**: More variance due to delayed attribution, budget shifts, and seasonality.  
- Platforms systematically **over-report** revenue.  

### 2. Modeled Revenue (Dev vs. Prod)
- Stable across environments, validating model assumptions.  
- Minor discrepancies (e.g., Bing, Pinterest, AdWords early prod phase) reflect real-world noise.  

### 3. Reported vs. Modeled Revenue
- Reported > Modeled across the board.  
- Modeled results are **stricter**, focusing on incremental impact rather than inflated totals.  

### 4. Incremental Revenue & ROI
- **Total ROI**: Reflects long-term performance of all spend.  
- **Marginal ROI**: Focuses on the **next dollar** — crucial for forward-looking budget allocation.  
- Channels with high historical ROI (e.g., Facebook, Amazon) may show **diminishing marginal returns**.  

### 5. Diminishing Returns on Spend
- Oversaturated channels yield weaker incremental ROI.  
- Modeled analysis highlights under-invested opportunities with higher marginal ROI.  

### 6. Lagged Effects
- Some channels show delayed impact (brand awareness), others react quickly.  
- Balancing short-term vs. long-term effects is key to portfolio allocation.  

### 7. Collinearity & VIF
- High correlation between channels (search + social) inflates credit.  
- Variance Inflation Factor (VIF) reveals **double-counting risks**.  
- The model mitigates this by assigning conservative contributions.  

---

## 🚀 Next Steps
Based on this work:
1. **Reallocate** spend away from saturated channels toward higher incremental ROI opportunities.  
2. **Experiment** with overlapping channels to optimize combinations.  
3. **Incorporate lag effects** into planning — balancing quick wins with long-term brand lift.  

---