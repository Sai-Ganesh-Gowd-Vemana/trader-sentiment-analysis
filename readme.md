# Trader Behavior vs Market Sentiment Analysis

## Overview

This project is about understanding how traders behave under different market sentiments like Fear and Greed.

The idea was simple — check whether sentiment actually affects trading performance, risk, and decision-making.

I worked with trading data and sentiment data, cleaned everything, merged it properly, and then analyzed patterns to find meaningful insights.

---

## What I Did

* Cleaned and prepared both datasets
* Converted timestamps and aligned data by date
* Merged sentiment with trading activity
* Created useful metrics like:

  * PnL
  * Win rate
  * Trade size
  * Drawdown proxy (losses)

Then I explored how these change across different sentiment conditions.

---

## Key Findings

* Traders perform best during **Extreme Greed**
* Performance drops during **Fear and Extreme Fear**
* Losses (drawdown proxy) are higher during volatile phases
* Traders take **larger risks during Fear**, which often backfires
* There is a clear behavioral pattern:

  * More buying during Fear
  * More selling during Greed

---

## Strategy Insights

Based on the analysis, a few simple takeaways:

* During Fear → reduce position size and avoid risky trades
* During Greed → focus on short-term profits and controlled exits
* Not all traders perform equally — weaker traders should avoid volatile conditions

---

## Model (Bonus)

I also built a simple model to predict next-day profitability.

* Used features like trade size and sentiment
* Removed data leakage properly
* Achieved around **62% accuracy**

This shows sentiment and behavior do have some predictive power, but more features can improve it.

---

## Project Structure

```
trader-sentiment-analysis/
│
├── data/
├── notebooks/
│   └── analysis.ipynb
├── outputs/
│   ├── charts
│   ├── tables
├── README.md
```

---

## How to Run

Clone the repo:

```
git clone https://github.com/Sai-Ganesh-Gowd-Vemana/trader-sentiment-analysis.git
```

Go to folder:

```
cd trader-sentiment-analysis
```

Install libraries:

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

Open notebook:

```
analysis.ipynb
```

---

## Final Thought

This project clearly shows that market sentiment has a strong impact on trading behavior and performance.

Even simple strategies based on sentiment can help reduce risk and improve decision-making.

---
