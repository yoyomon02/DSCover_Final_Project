# ⚾ Kiwoom Heroes: Data-Driven Team Revitalization Strategy

**2025-2 DScover Main Project(Grand Prize - 1st Place)**

## 📌 Project Overview

The Kiwoom Heroes have faced significant performance declines in recent seasons. This project employs a data-driven approach to identify the team's core structural weaknesses and propose a mathematically optimized recruitment strategy for the 2026 KBO season. By combining multivariate regression, Pythagorean expectation, and Monte Carlo simulations, we forecast a path from a projected 40-win season to a competitive 50+ win baseline.

## 📊 Data Sources
**Performance Data:** 2021–2025 player and team statistics for Kiwoom and the wider KBO (Source: Baseball Reference).
 
**FA Market Data:** 10 years of Free Agent market historical data (Source: KBO Press Releases).

**Financial Data:** 5-year financial state and audit reports of the Kiwoom Heroes (Source: Kiwoom Heroes Audit Reports).


## ⚙️ Methodology

### 1. Data Processing & EDA

**Cleaning:** Handled missing values through logical recalculation (e.g., W-L%) and zero-filling for relevant baseball metrics.

**Correlation Analysis:** Identified key drivers of team rank, finding high correlations between rank and **OBP** () for batters and **RA9** () for pitchers.


### 2. Custom Performance Scoring

To evaluate players objectively, we developed custom scoring models based on multivariate regression:

**Batting Score:** Based on **wOBA** (weighted On-Base Average), accounting for the specific run-scoring value of BB, 1B, 2B, 3B, and HR.

**Pitching Score:** Based on **RA9** impact, analyzed separately for Starting Pitchers (SP) and Relief Pitchers (RP) to account for different usage patterns.


### 3. 2026 Season Simulation

**Algorithm:** Utilized **Pythagorean Win Percentage** to convert projected runs scored (RS) and runs allowed (RA) into winning probabilities.

**Monte Carlo Simulation:** Ran **10,000+ iterations** to account for seasonal volatility, injuries, and "luck" factors to generate a statistically sound win-mean and confidence intervals.



### 4. Financial & Recruitment Optimization

**Budgeting:** Analyzed Kiwoom's lean financial structure and projected a **6.4 billion KRW** budget (12% of revenue) for the 2025/2026 stove league.

**FA Analysis:** Visualized the impact of prospective FA acquisitions (e.g., Choi Hyoung-woo, Kim Tae-hun) on the team's overall scoring profile.



## 📈 Key Results

**Baseline Forecast:** Before recruitment, the 2026 model predicted a last-place finish with approximately **37–40 wins**.

**Post-Recruitment Forecast:** With strategic FA signings targeting high-impact batters and relief pitching, simulations show a significant jump to **50+ wins**.

## 🛠 Tech Stack

* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn
**AI Simulation:** Google AI Studio (Gemini 1.5 Pro) for prompt engineering-based season modeling.
