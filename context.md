# Project Context: AI-Powered CSV Forecaster

## 1. Project Overview

This is a single-page web application built with vanilla HTML, CSS, and JavaScript (`index.html`). The application serves as an "AI-Powered CSV Forecaster."

**Core Functionality:**
- Users upload a CSV file containing time-series data.
- Users provide their Google Gemini API key.
- The application processes the data through a pipeline of four specialized AI agents to produce an analysis, forecast, and summary.

**Technologies Used:**
- **Frontend:** HTML, Tailwind CSS
- **JavaScript:** Vanilla JS (ES Modules), Chart.js (for charts), jQuery/DataTables (for tables)
- **AI:** Google Gemini API

## 2. Current AI Agent Logic

The application employs a multi-agent system where data is passed sequentially:

- **Agent 1 (Data & Table Generator):** Takes the raw CSV, cleans it, and outputs both clean JSON data and an HTML table for display.
- **Agent 2 (Forecasting Specialist):** Takes the clean JSON data and generates a 30-period forecast.
- **Agent 3 (Reasoning Analyst):** Takes the historical and forecast data and generates a rationale explaining the forecast.
- **Agent 4 (Reporting Analyst):** Takes all the data and the rationale to create a final executive summary.

## 3. User's Goal: Refine Agent Logic

The user wants to align the agent workflow with a more intuitive, human-like analytical process. The desired flow is as follows:

1.  **CSV -> Generate Table:** The initial CSV is used to generate a data table.
2.  **Table -> Generate Forecast Chart:** The generated table is used as the basis for creating a forecast chart.
3.  **Chart -> Generate Forecast Explanation:** The generated chart is analyzed to produce an explanation of the forecast.
4.  **Table + Chart -> Generate ERP Pro Summary:** A final, powerful summary is created by synthesizing information from both the table and the chart.

## 4. Proposed Implementation Plan

The current system is efficient because it passes structured JSON data between agents rather than having them parse visual HTML tables or chart images.

To meet the user's goal without sacrificing this efficiency, the plan is to **modify the prompts** of the agents to make them "act" as if they are analyzing the visual components.

**Specific Change:**
- **Modify Agent 4's Prompt:** The prompt for the final agent will be updated to explicitly state that it should analyze the "provided data table and forecast chart" to generate its "powerful ERP pro summary."
- **Data Framing:** The data sent to Agent 4 will be structured to reinforce this framing (e.g., labeling the data as `dataForTable` and `dataForChart`).

This approach aligns the agent's behavior and output with the user's vision while maintaining the robust, data-driven backend.
