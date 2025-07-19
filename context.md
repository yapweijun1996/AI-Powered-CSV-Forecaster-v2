# AI-Powered CSV Forecaster Context

This project is an AI-powered CSV data analysis and forecasting tool designed to provide instant insights, forecasts, and visualizations from uploaded CSV files. It leverages a team of specialized AI agents, each with a distinct role, to process data, generate forecasts, explain reasoning, and produce executive summaries.

## AI Agents and Their Roles

- **Agent 1 (Data & Table Generator):**  
  A professional ERP data specialist responsible for cleaning raw CSV data by accurately identifying the primary date/time and numerical value columns. Generates a well-formatted, accessible HTML table adhering to enterprise UI standards.

- **Agent 2 (Forecasting Specialist):**  
  A professional forecasting expert who rigorously evaluates and refines initial statistical forecasts based on historical data. Ensures forecasts are analytically sound, align with business trends, and produce realistic, data-driven projections.

- **Agent 3 (Reasoning Analyst):**  
  A professional data reasoning analyst who provides clear, concise, and authoritative explanations of forecast logic. Analyzes trends such as growth, seasonality, and anomalies, delivering insights suitable for senior management.

- **Agent 4 (Reporting Analyst):**  
  A senior ERP professional reporting analyst tasked with synthesizing data tables, forecasts, and rationale into a polished, cohesive executive summary. The summary is designed for high-level ERP system reports and actionable business insights.

## Technical Details

- Uses Google Gemini API for AI model interactions.
- Employs Chart.js for data visualization with dual charts: statistical forecast and AI-validated forecast.
- Implements client-side statistical forecasting using simple-statistics linear regression.
- Utilizes IndexedDB for API key persistence.
- Provides interactive data tables with DataTables.js.
- Supports multiple output languages for AI-generated content.

## Professionalism and Context Engineering

The AI agent prompts have been carefully engineered to reflect professional personas typical of staff at leading ERP companies. This ensures outputs are precise, rigorous, and business-appropriate, enhancing the credibility and usefulness of the forecasts and reports generated.
