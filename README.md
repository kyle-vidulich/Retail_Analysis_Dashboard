Retail Performance Analytics Dashboard
Overview
This project analyzes four years of retail transaction data to give leadership a clear, decision-ready view of sales performance, profit drivers, geographic trends, and discount sensitivity. Built in Tableau Public with a two-agent CrewAI workflow that automatically extracts verified findings and delivers an executive-ready email to retail leadership.

Tools

Tableau Public -- dashboard design, interactive filtering, forecasting, and What-If scenario modeling
CrewAI -- two-agent agentic AI workflow for automated analysis and executive communication


Dataset
Four years of retail transaction data (2020-2023) across three joined tables: Sales Data, Regional Manager, and Zip Code. Key fields include Total Sales, Total Profit, COGS, Customer Segment, Product Category, Sub-Category, Order Date, and Geography. Calculated fields built in Tableau include CY Sales, PY Sales, Sales Percent Change, Adjusted Profit, and an Arrow Indicator.

Dashboard Features

Five interactive charts covering sales KPIs, category performance, geographic profit, forecasting, and discount scenario modeling
Dynamic filtering by Month, Region, and Segment applied simultaneously across all charts
Discount Rate parameter enabling real-time What-If scenario analysis at any discount threshold
AI-powered recommendations panel embedded directly in the dashboard
CY Selection parameter allowing leadership to toggle between fiscal years dynamically


Key Findings

2023 peaked at $121K in November, the highest single month across all four years, but December reversed sharply below prior year for the first time -- a signal worth monitoring heading into 2024
Tables is the most critical sub-category in the portfolio -- generating $207K in revenue while confirmed losing -$18K in total profit, deepening to -$28K at a 5% discount rate
Texas is the single worst-performing state at -$26K confirmed total profit loss, while California ($76K) and New York ($74K) are the two strongest profit markets in the country
Forecast model achieved a MASE of 0.59 -- 41% more accurate than a naive baseline estimate -- with February and October confirmed as consistent annual revenue dip points across all four years


Strategic Recommendations

Enforce a sub-category discount approval policy with Tables, Bookcases, Supplies, and Machines on a hard no-discount list, while targeting Copiers, Paper, and Envelopes as the strongest candidates for promotional discounting
Reallocate regional investment toward California and New York and pause discretionary spend in Texas (-$26K), Ohio (-$17K), and Pennsylvania (-$16K) until root cause of losses is identified
Deploy targeted promotions in February and October to offset confirmed repeating annual revenue dips, supported by a forecast model carrying a MASE of 0.59


CrewAI Workflow
The project includes a two-agent CrewAI workflow named RetailAnalytics_AgenticAI. Agent 1, the Retail Analytics Specialist, reads the Analytics Context Summary PDF and extracts only verified findings grounded in Tableau data. Agent 2, the Business Strategy Advisor, reasons through those findings and drafts an executive-ready email for retail leadership and the VP of Operations covering the three main findings, three recommendations, and one key caution. Agent output was evaluated against verified Tableau data -- the agent performed well on profit and geographic findings but omitted forecast insights and lacked nuance in recommendations, reinforcing the importance of human review before acting on any AI-generated output.

Business Hypotheses Tested
Hypothesis: Sub-categories discounted above baseline threshold generate lower profit margins regardless of sales volume - Supported
At least one region performs significantly below company average profit - Supported
Highest revenue segment shows flat or negative profit growth indicating growth is bought not earned - Contradicted

<img width="2865" height="1634" alt="Screenshot 2026-05-06 194414" src="https://github.com/user-attachments/assets/9e932312-7f0f-47c4-97aa-7b2c034d163e" />


         
