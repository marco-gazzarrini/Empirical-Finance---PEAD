# Does Betting on Standardized Unexpected Earnings Still Work?
### Revisiting the Post-Earnings Announcement Drift (PEAD)

**Course:** Empirical Finance – Católica Lisbon School of Business and Economics  
**Authors:** Marco Gazzarrini, Alexandre Rocha, Bruno Morais,  Riccardo Berruti, Severin Blumenthal  
**Supervisors:** José Faias, Zoë Venter

---

## Overview

This paper revisits the Post-Earnings Announcement Drift (PEAD) anomaly originally 
documented by Bernard & Thomas (1989), asking whether it remains exploitable in 
modern financial markets.

Using firm-level data from CRSP and IBES covering **~14,000 U.S. tickers** 
(NYSE, NASDAQ, AMEX) between **2004 and 2023**, we construct SUE-based 
long-short portfolios and measure Cumulative Abnormal Returns (CAR) over a 
60-trading-day window following each earnings announcement.

---

## Research Questions

1. Does PEAD still exist in modern financial markets?
2. Does the drift vary by firm size (small-, mid-, large-cap)?
3. Are certain industry sectors more prone to this anomaly?

---

## Methodology

- **SUE construction:** 24-period rolling regression to forecast EPS; SUE 
  winsorized at 1st/99th percentiles
- **Portfolio formation:** Stocks ranked into deciles by SUE each quarter; 
  long D10 (top), short D1 (bottom)
- **CAR measurement:** Market-adjusted model, 60-day event window, 
  ~388,000 CAR observations
- **Statistical tests:** Two-sided t-test on annualized returns; Sharpe ratio 
  computed for each sub-portfolio
- **Tool:** Stata

---

## Key Findings

| Segment | Result |
|---|---|
| Full sample (all stocks) | No statistically significant abnormal returns |
| Small-cap | Negative returns (contradicts prior literature) |
| **Large-cap** | **+0.96% mean return, statistically significant (p=0.04)** |
| HiTech, Manufacturing, Shops | Positive and significant long-short returns (~2.8%) |
| Utilities, Other | Significant negative returns |

> **Main conclusion:** PEAD is no longer broadly exploitable, but persists 
> selectively in large-cap stocks and specific sectors — a structural shift 
> from the small-cap dominance documented in the 1980s.

---

## Repository Contents

- `EF Final Project.pdf` – Full report including methodology, results, and discussion

---

## References

- Bernard & Thomas (1989) – *Post-Earnings-Announcement Drift: Delayed Price Response or Risk Premium?*
- Livnat & Mendenhall (2006) – *Comparing the Post-Earnings Announcement Drift for Surprises Calculated from Analyst and Time Series Forecasts*
