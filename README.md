# 📊 Quant Research Note

## Trader Performance vs Market Sentiment

---

## 1. Executive Summary

This study examines how market sentiment—proxied by the Fear & Greed Index—impacts trader behavior and performance.

**Key Result:**
Trader profitability is not purely a function of market direction, but of **behavioral adaptation to sentiment regimes**.

* **Fear regimes** → Higher-quality trades, improved PnL stability
* **Greed regimes** → Increased activity, higher risk, unstable returns

**Core Insight:**

> Markets reward discipline during uncertainty and penalize overconfidence during bullish sentiment.

---

## 2. Research Objective

To quantify the relationship between:

* Market sentiment (Fear vs Greed)
* Trader behavior (frequency, size, aggression)
* Trading performance (PnL, win rate, variability)

---

## 3. Data Description

### Trading Dataset

* ~5000 trade-level records
* Fields include:

  * Account-level activity
  * Trade size (USD)
  * Direction (Buy/Sell)
  * Closed PnL
  * Timestamp (IST)

### Sentiment Dataset

* ~2000 daily observations
* Fear & Greed classification
* Aligned to trading dates

---

## 4. Methodology

### 4.1 Data Preparation

* Standardized column names
* Converted timestamps to daily granularity
* Aligned sentiment with trading data

### 4.2 Feature Engineering

Constructed trader-day level metrics:

* **Daily PnL** → Profitability
* **Trade Count** → Activity level
* **Average Trade Size** → Risk exposure
* **Win Rate** → Execution efficiency
* **Aggression** = Trade Size × Frequency
* **Long Ratio** → Directional bias

### 4.3 Analytical Framework

* Sentiment-based grouping
* Behavioral segmentation
* Distributional analysis (not just averages)

---

## 5. Key Findings

### 5.1 Sentiment vs Profitability

* Fear regimes show **higher and more consistent PnL**
* Suggests:

  * Reduced noise
  * More selective participation
  * Better opportunity asymmetry

---

### 5.2 Behavioral Shift in Greed

* Trade frequency ↑
* Trade size ↑
* Aggression ↑

**Interpretation:**
Greed induces **overconfidence-driven trading**, leading to inefficiencies.

---

### 5.3 Overtrading Effect

* High-frequency traders exhibit **lower average profitability**

**Implication:**

> Increased activity does not translate to increased edge.

---

### 5.4 Risk vs Return Asymmetry

* Greed periods show:

  * Higher variance in PnL
  * Lower consistency

**Conclusion:**
Returns during Greed are **risk-driven, not skill-driven**.

---

## 6. Behavioral Segmentation Insights

| Segment         | Behavior            | Outcome           |
| --------------- | ------------------- | ----------------- |
| Low Frequency   | Selective trading   | Higher efficiency |
| High Frequency  | Overtrading         | Reduced returns   |
| Low Aggression  | Controlled exposure | Stable PnL        |
| High Aggression | Risk-heavy trades   | Volatile outcomes |

---

## 7. Strategic Implications

### 7.1 Capital Allocation Strategy

* Increase exposure during **Fear regimes**
* Focus on high-conviction setups

---

### 7.2 Risk Management Framework

* Enforce position limits during **Greed**
* Reduce leverage and trade size

---

### 7.3 Behavioral Controls

* Implement trade frequency caps
* Monitor aggression metrics as risk signals

---

### 7.4 System-Level Insight

> Performance degradation is primarily behavioral—not informational.

---

## 8. Limitations

* No transaction cost modeling
* No latency/slippage consideration
* Trader skill heterogeneity not isolated

---

## 9. Future Work

* Regime-based predictive modeling
* Clustering traders by behavioral profiles
* Incorporating volatility and liquidity signals
* Sharpe-like risk-adjusted performance metrics

---

## 10. Tools & Stack

* Python (Pandas, NumPy)
* Visualization (Seaborn, Matplotlib)
* Jupyter Notebook

---

## 11. Author

--SANJAY KUMAR S
Data Science & Quantitative Analysis

---

## Final Note

This analysis reinforces a core principle in trading systems:

> **Edge is not only informational—it is behavioral.**
