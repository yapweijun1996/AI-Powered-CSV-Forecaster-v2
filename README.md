# AI-Powered CSV Forecaster

This project is a web-based tool that uses a team of AI agents to analyze, forecast, and visualize data from a CSV file. It's designed to be easy to use: just upload a file, and the AI team will deliver a comprehensive report, including an interactive data table, a multi-chart dashboard, and a detailed summary.

## Features

-   **AI-Powered Analysis:** Leverages the Google Gemini API to perform sophisticated data analysis and forecasting.
-   **Multi-Agent System:** A team of specialized AI agents work together, each handling a specific task like data cleaning, forecasting, or reporting.
-   **Dynamic Visualizations:** Automatically generates a dashboard with multiple charts (lines, bars, etc.) using Chart.js to best represent your data.
-   **Interactive Data Table:** Displays your cleaned data in a searchable and sortable table using DataTables.js.
-   **Customizable Models:** Choose between different AI models (Gemini 2.5 Flash or Pro) for each agent to balance speed and power.
-   **No Backend Required:** The entire application runs directly in your web browser.

## How to Use

This project is a single HTML file and requires no complex setup. Here’s how to get it running:

### Step 1: Get a Google Gemini API Key

The AI agents need an API key to work.

1.  Go to the [Google AI Studio](https://aistudio.google.com/) website.
2.  Sign in with your Google account.
3.  Click on **"Get API key"** and then **"Create API key in new project"**.
4.  Copy the key that is generated. It will be a long string of letters and numbers.

### Step 2: Open the Application

1.  Find the `index.html` file in the project folder.
2.  Right-click on it and choose **"Open with"** your favorite web browser (like Chrome, Firefox, or Edge). You can also simply drag the file into an open browser window.

### Step 3: Run an Analysis

Once the page is open in your browser, follow these steps:

1.  **Paste Your API Key:** In the "Google Gemini API Key" field, paste the key you got from Google AI Studio.
2.  **Upload a CSV File:** Click the upload area and select a CSV file from your computer. The file should have at least one column with dates or time-based labels and one column with numbers.
3.  **Configure (Optional):** You can change the output language or select different AI models for each agent. The default settings are fine for your first run.
4.  **Click "Analyze Data":** The button will become active once you've provided an API key and a file. Click it to start the process.

The AI agents will now begin their work. You will see status updates as they complete their tasks, and the final report will appear on the page.

## How It Works: The AI Team

This project uses a "multi-agent" approach. Think of it as a team of AI specialists, where each one has a specific job.

1.  **Data Cleaner:** Takes your raw CSV file, cleans it up, and organizes it into a clean table.
2.  **Forecasting Specialist:** Looks at the historical data and creates a data-driven forecast for the future.
3.  **Reasoning Analyst:** Explains *why* the forecast looks the way it does, based on trends in the data.
4.  **Reporting Analyst:** Writes a professional, high-level summary of all the findings.
5.  **Chief Visualization Officer:** The creative lead. This agent designs a dashboard of multiple charts to tell a compelling story with your data.

This approach allows each AI to focus on what it does best, leading to a higher-quality final report.

## Technologies Used

-   **HTML5**
-   **Tailwind CSS:** For styling the user interface.
-   **JavaScript:** For all the application logic.
-   **Google Gemini API:** The AI engine powering the agents.
-   **Chart.js:** For creating the charts and dashboard.
-   **DataTables.js:** For the interactive data table.
-   **Marked.js:** For rendering the final summary (which is written in Markdown).
-   **simple-statistics:** For the initial, basic statistical forecast.
