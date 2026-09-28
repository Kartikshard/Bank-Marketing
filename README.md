from pathlib import Path

readme = r"""# 🏦 Bank Marketing Campaign Intelligence

<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0f172a,50:2563eb,100:06b6d4&height=180&section=header&text=Bank%20Marketing%20ML&fontSize=42&fontColor=ffffff&animation=fadeIn&fontAlignY=35" width="100%"/>
</p>

<p align="center">
  <strong>Predicting term-deposit subscriptions and turning ML probabilities into actionable campaign decisions.</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.x-3776AB?style=for-the-badge&logo=python&logoColor=white"/>
  <img src="https://img.shields.io/badge/Pandas-2.x-150458?style=for-the-badge&logo=pandas&logoColor=white"/>
  <img src="https://img.shields.io/badge/scikit--learn-ML-F7931E?style=for-the-badge&logo=scikit-learn&logoColor=white"/>
  <img src="https://img.shields.io/badge/Power%20BI-Dashboard-F2C811?style=for-the-badge&logo=powerbi&logoColor=black"/>
  <img src="https://img.shields.io/badge/Status-Completed-22C55E?style=for-the-badge"/>
</p>

---

## 🎯 The Business Question

> **Which customers should the bank prioritize for a marketing call?**

A bank's sales team has limited time and every unnecessary call consumes resources.

Instead of treating every customer equally, this project builds a machine-learning system that estimates each customer's probability of subscribing to a **term deposit** and converts that probability into a business decision.

```text
                         🏦 BANK
                            │
                            ▼
                    4,521 CUSTOMERS
                            │
                            ▼
                  ┌───────────────────┐
                  │ ML MODEL          │
                  │                   │
                  │ Subscription      │
                  │ Probability       │
                  └─────────┬─────────┘
                            │
                            ▼
                    Business Threshold
                         0.37
                       ╱       ╲
                      ╱         ╲
                 < 0.37       ≥ 0.37
                    │             │
                    ▼             ▼
                 DON'T         PRIORITIZE
                 CALL             CALL
