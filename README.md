<img width="1063" height="712" alt="image" src="https://github.com/user-attachments/assets/a24051db-83f8-49c8-b12a-65ca88e388ba" /># ecom-consumer-demographics-analytics

# Enterprise Consumer Demographics & Behavioral Analytics

A comprehensive data analytics repository engineered to process customer profiles, track transaction frequencies, and extract consumer purchasing patterns. This project combines exploratory data analysis (EDA), automated data cleaning pipelines, and customer segmentation matrices to deliver actionable marketing intelligence and optimize lifetime account value.

---

## 1. Executive Summary & Core Volume Ledgers

An audit of our active consumer database establishes a clear, real-time tracking reference framework for business operations:

*   **Total Customer Base:** 10,675 unique customer profiles processed within the analytics pipeline.
*   **Regional Geographic Footprint:** Active consumer accounts mapped across 10 distinct US states.
*   **Behavioral Tracking Matrix:** Core analysis tracking demographic features against monthly spending values and customer engagement timelines (Days Since Last Interaction).

<div align="center">
  <img src="https://private-user-images.githubusercontent.com/50950725/659449693-5ad6f3fc-885a-4e3b-907b-8a5ab0fcf050.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3OTA0MzYzNTksIm5iZiI6MTc5MDQzNjA1OSwicGF0aCI6Ii81MDk1MDcyNS82NTk0NDk2OTMtNWFkNmYzZmMtODg1YS00ZTNiLTkwN2ItOGE1YWIwZmNmMDUwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA5MjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwOTI2VDE1MjA1OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTlmNGI3MGI3YjY5YTlkOGMzYjgyNzNmMzZmZTdmYTNiZWRjNzBlY2FiMGQ1ZjYwZmExNDhkOWFlOGRhMmVjYWEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JnJlc3BvbnNlLWNvbnRlbnQtdHlwZT1pbWFnZSUyRnBuZyJ9.Shgh7JW_X6sAGcdCq_BAeT_Io1XetBj2DfhwrpU_zcw" width="32%" alt="Age Distribution Matrix" />
  <img src="https://private-user-images.githubusercontent.com/50950725/659449690-dd79c547-0184-42f5-be76-1527089b7358.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3OTA0MzYzNTksIm5iZiI6MTc5MDQzNjA1OSwicGF0aCI6Ii81MDk1MDcyNS82NTk0NDk2OTAtZGQ3OWM1NDctMDE4NC00MmY1LWJlNzYtMTUyNzA4OWI3MzU4LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA5MjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwOTI2VDE1MjA1OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWU4MWE5ODg2NTQzZmU4Zjg1NzIyMWNhNzk0MGI4MTBjODA1OGQ1ZGUyNzI5MWE1MmU3ZDNhMmFmOWQ1NThiYjAmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JnJlc3BvbnNlLWNvbnRlbnQtdHlwZT1pbWFnZSUyRnBuZyJ9.Sg3Jg3PGoq6NFbentwCFI9DK2dXpY7Lz-ciSP0IYV2A" width="32%" alt="Monthly Spend Outlier Vector" />
  <img src="https://private-user-images.githubusercontent.com/50950725/659449696-ec6e285a-ed73-4df4-9745-d2d1e51c7830.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3OTA0MzYzNTksIm5iZiI6MTc5MDQzNjA1OSwicGF0aCI6Ii81MDk1MDcyNS82NTk0NDk2OTYtZWM2ZTI4NWEtZWQ3My00ZGY0LTk3NDUtZDJkMWU1MWM3ODMwLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA5MjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwOTI2VDE1MjA1OVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWZmMmNhNzVkNTM3MzM1MjBhODQyMjM1N2YxZTlhMTk4N2NmZDgzZmExNDMzYjdjZTQ2MTQ0M2RhODllYjI0ZDMmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JnJlc3BvbnNlLWNvbnRlbnQtdHlwZT1pbWFnZSUyRnBuZyJ9.FXWeiht_WGpZ8HL6fQDvMew6CAJRXeEBTf5k6yA7mpM" width="32%" alt="Categorical Base Breakdown" />
</div>

---

## 2. Project Directory Structure

The repository files are organized according to clean production standards:

```text
ecom-consumer-demographics-analytics/
│
├── data/
│   └── us_consumer_profiles.csv  # Verified master consumer dataset
│
├── consumer_spend_analytics.ipynb       # Exploratory Python analytics notebook
└── consumer_behavior_executive_report.pdf # Ready-to-read executive data report
```

---

## 3. Multi-Variate Spend Features & Correlation Ledgers

To map the relationships between customer attributes and spending volumes, the pipeline processes multi-variate continuous plots and linear covariance heatmaps:

<div align="center">
  <img src="https://private-user-images.githubusercontent.com/50950725/659449697-a621ff70-bc55-4842-82df-44b67bc48085.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3OTA0MzY2MDQsIm5iZiI6MTc5MDQzNjMwNCwicGF0aCI6Ii81MDk1MDcyNS82NTk0NDk2OTctYTYyMWZmNzAtYmM1NS00ODQyLTgyZGYtNDRiNjdiYzQ4MDg1LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA5MjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwOTI2VDE1MjUwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTVhNDEzNjhiZDliMTY3MmIyYmI0Nzc2YzI5ZjVjYWE0MDdlODMxYTliNDI3N2VmMTAwY2Y0NTQ0MDNiNDdlN2YmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JnJlc3BvbnNlLWNvbnRlbnQtdHlwZT1pbWFnZSUyRnBuZyJ9.FOkGgSOVSgBe6Cfxp_6U98jP1Bdx_o4IcjW78osNOE0" width="32%" alt="Orthogonal Spend Vector" />
  <img src="https://private-user-images.githubusercontent.com/50950725/659449689-bb5ed1cd-9f87-4dab-9617-0fd6c8bd0222.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3OTA0MzY2MDQsIm5iZiI6MTc5MDQzNjMwNCwicGF0aCI6Ii81MDk1MDcyNS82NTk0NDk2ODktYmI1ZWQxY2QtOWY4Ny00ZGFiLTk2MTctMGZkNmM4YmQwMjIyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA5MjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwOTI2VDE1MjUwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTBhYjRkZTRkM2UxMjY0MTRiMGJkOGQ5MzkxMjAxZWUzMjUxMDI0Y2YzMjgyNGRlNTgxNDQ5ZGYzZWRmYzY0YjEmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JnJlc3BvbnNlLWNvbnRlbnQtdHlwZT1pbWFnZSUyRnBuZyJ9.XjBX_CCyzBN7OPDrE2urnmt41Q177enesTSChh5hR5Y" width="32%" alt="Multi-Class Density Waves" />
  <img src="(https://private-user-images.githubusercontent.com/50950725/659449694-0718de6f-5219-4594-a6c9-25eaf93eadb1.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3OTA0MzY2MDQsIm5iZiI6MTc5MDQzNjMwNCwicGF0aCI6Ii81MDk1MDcyNS82NTk0NDk2OTQtMDcxOGRlNmYtNTIxOS00NTk0LWE2YzktMjVlYWY5M2VhZGIxLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA5MjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwOTI2VDE1MjUwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTYxYzEyNDQ4OTY5NjIwODZmY2M2ZDc1YjVmOGVlNjk4YzBmNjM0NjE2ZTllYTcyMTA5NmI3ZDQ5NjExNTZiZWQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JnJlc3BvbnNlLWNvbnRlbnQtdHlwZT1pbWFnZSUyRnBuZyJ9.UYYLeBC4chNSHDrf5YvEDTLldOK5YYfwtBPtL06MDWs" width="32%" alt="Linear Covariance Matrix" />
</div>

*   **The Orthogonality Finding:** Our correlation metrics reveal near-zero linear relationships across every feature indicator (e.g., Age vs. MonthlySpend = -0.01). 
*   **Outlier Retention Anomalies:** While the baseline portfolio clusters heavily inside the lower budget band (\$100 to \$500), the distribution model flags a dense trail of high-value premium anomalies stretching up to \$1,750.

---

## 4. Inferential Statistics Ledger & Strategic Recommendations

To ensure marketing allocations are backed by mathematical proof rather than guesswork, the pipeline runs extensive parametric testing across all customer cohorts:

<div align="center">
  <img src="https://private-user-images.githubusercontent.com/50950725/659449692-b02157fd-f9e3-4c0d-96b4-c0415828b901.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3OTA0MzY2MDQsIm5iZiI6MTc5MDQzNjMwNCwicGF0aCI6Ii81MDk1MDcyNS82NTk0NDk2OTItYjAyMTU3ZmQtZjllMy00YzBkLTk2YjQtYzA0MTU4MjhiOTAxLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA5MjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwOTI2VDE1MjUwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTY0ZjdjNmMwZmU2NDdkNDIyMGRmZTc1MjEzZDUyODgxM2M2M2RlNDQxOGNmMmM2M2MxMzA2NjkwNTA3ZWZmYzYmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JnJlc3BvbnNlLWNvbnRlbnQtdHlwZT1pbWFnZSUyRnBuZyJ9.gdxLx7JATOmZn12eBbilMQT10SlgyVK-A8QrjqVyFyA" width="100%" alt="State-Wise Distribution Matrix" style="margin-bottom: 15px;" />
  <br>
  <img src="https://private-user-images.githubusercontent.com/50950725/659449691-02cb160e-52d6-46aa-ad2f-dbb6c368f592.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3OTA0MzY2MDQsIm5iZiI6MTc5MDQzNjMwNCwicGF0aCI6Ii81MDk1MDcyNS82NTk0NDk2OTEtMDJjYjE2MGUtNTJkNi00NmFhLWFkMmYtZGJiNmMzNjhmNTkyLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA5MjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwOTI2VDE1MjUwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTQxODhiZGYwMGM5YTZmZDc4YWY1ZTFmNTZjZWQ2YTc5Y2Y4N2VhZDYxMzJhNGZjZGIyODVlM2E3MWU0YjYyODQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JnJlc3BvbnNlLWNvbnRlbnQtdHlwZT1pbWFnZSUyRnBuZyJ9.WglY0HX2oLdY9iY_7-lsPOGD81CxvMVy6JlR6ieAsG8" width="100%" alt="Master Insights Registry" style="margin-bottom: 15px;" />
  <br>
  <img src="(https://private-user-images.githubusercontent.com/50950725/659449695-b4d9d61c-2106-4a41-a811-84163325fe1c.png?jwt=eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3OTA0MzY2MDQsIm5iZiI6MTc5MDQzNjMwNCwicGF0aCI6Ii81MDk1MDcyNS82NTk0NDk2OTUtYjRkOWQ2MWMtMjEwNi00YTQxLWE4MTEtODQxNjMzMjVmZTFjLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNjA5MjYlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjYwOTI2VDE1MjUwNFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPWVlODg2ZDdlZTVlNGQ1ZjA1MGMyNWY1OTFjYWYwZDdmNDExM2Q3MThhYWEyYTAxMWY0MGMzNGQyZTM2MzhlYWQmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JnJlc3BvbnNlLWNvbnRlbnQtdHlwZT1pbWFnZSUyRnBuZyJ9.AMfk9ZpJ9sgfXnAC61-rMGg8scn9Qcsgn6F6rkFZjkM" width="100%" alt="Repository Root Alignment" />
</div>

### Core Strategic Business Insights
1.  **Uniform Customer Spending:** Our Independent t-tests and One-Way ANOVA models successfully accepted the Null Hypothesis ($H_0$), logging exceptionally high p-values across Gender ($p = 0.7345$), Education ($p = 0.9224$), and State ($p = 0.3457$).
2.  **Marketing Cost Reductions:** Because purchasing behavior remains uniform across all demographics, the business can completely avoid costly segment-specific advertising campaigns. Resources can be safely consolidated into broad, high-budget national marketing distributions to maximize reach while lowering overhead.
3.  **Generational Interaction Tuning:** The correlation coefficient between customer age and interaction timelines is practically non-existent ($r = -0.0040$). Churn prevention alerts, automated win-back emails, and interaction triggers should be applied identically across all age groups.

---

## 5. Deployment Architecture

*   **Data Aggregation Core:** Engineered entirely within a Jupyter Notebook pipeline using Python.
*   **Data Manipulation Toolkits:** Managed using Pandas dataframes and NumPy array select structures.
*   **Visual Presentation Graphics:** Rendered using Matplotlib and Seaborn plotting engines.
