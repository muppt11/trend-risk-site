# TrendRisk

**Live demo: https://muppt11.github.io/trend-risk-site/**

A production order planner for fashion brands. A planner has to commit to an order before they know if demand will hold. TrendRisk takes their demand forecast and supplier lead times and tells them, with reasons, whether the order is safe to release, risky, or needs a faster supplier.

## What it does

- Turns company inputs and supplier lead times into a production window using plain, deterministic math
- Flags risk and explains exactly why, so nothing is a black box
- Compares scenarios side by side, like a supplier delay versus a faster shipping option
- Accepts CSV or Excel inputs, saves scenarios, and builds baselines from sales history
- Includes a guided 3 to 5 minute demo with presenter notes

Everything runs in the browser. Your inputs never leave your computer.

## Challenges

**Making a risk score people trust.** A planner won't act on a number they can't explain to their boss. I kept the math deterministic and show the reasoning next to every flag instead of using a model that just outputs a score.

**Demoing without real customer data.** Real order data is private. The demo uses clearly labeled synthetic orders, and the sales baseline comes from the public UCI Online Retail dataset (CC BY 4.0), so the numbers behave realistically without exposing anyone.

**Keeping it private by default.** Brands don't want to upload supplier data to a stranger's server, so I shipped it as a static site where all calculations happen locally.

## About this repo

This repo holds the published static build that GitHub Pages serves. Data credit: Daqing Chen, UCI Online Retail, https://doi.org/10.24432/C5BW33.
