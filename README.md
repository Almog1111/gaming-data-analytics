# Mobile Game In-App Purchases — Data Analytics

## Project Overview

This project analyzes mobile game player behavior, in-app purchases, and revenue distribution to identify business insights that can support data-driven decision-making.

The analysis covers 3,024 player records and combines Python-based exploratory data analysis, business intelligence dashboards, and AI-assisted interactive analytics.

The project was developed as part of a Junior Data Analyst portfolio.

## Live Interactive Dashboards

**Explore the dashboards directly in your browser — no downloads or installations required.**

### 1. Mobile Game In-App Purchases — Analytics Dashboard

[▶ Open Live Analytics Dashboard](https://almog1111.github.io/gaming-data-analytics/dashboards/Mobile%20Game%20In-App%20Purchases%20%E2%80%94%20Analytics%20Dashboard.html)

Explore recorded revenue, player spending segments, age groups, game genres, countries, engagement metrics, and data limitations through interactive charts and filters.

### 2. Device Type vs Recorded Spending — Ad-hoc Analysis

[▶ Open Live Device Analysis](https://almog1111.github.io/gaming-data-analytics/dashboards/Device%20Type%20vs%20Recorded%20Spending%20%E2%80%94%20Ad-hoc%20Analysis.html)

Compare recorded spending across device types and spending segments using interactive visualizations and descriptive statistical comparisons.

**[Browse the dashboards folder](https://github.com/Almog1111/gaming-data-analytics/tree/main/dashboards)** for the dashboard files and their launch links.

> **Note:** GitHub displays HTML files as source code. Use the live dashboard links above to open the interactive versions.

## Business Objectives

The project focuses on five business questions:

1. How is recorded revenue distributed across player spending segments?
2. Which age groups contribute the most recorded revenue?
3. How does revenue vary across game genres?
4. How concentrated is revenue across countries?
5. How does player engagement differ between spending segments?

An additional AI-assisted analysis explores recorded spending differences between device types.

## Tools and Technologies

- **Python:** Data analysis and calculations.
- **Pandas:** Data cleaning, grouping, aggregation, and exploratory analysis.
- **Matplotlib:** Data visualization.
- **Jupyter Notebook:** Analytical workflow and documentation.
- **Power BI:** Interactive business intelligence dashboard.
- **Claude AI:** Independent analytical review and generation of interactive dashboards from natural-language requests.

## Dataset

The dataset contains **3,024 player records and 13 original columns**.

The available information includes:

- **Player demographics:** age, gender, and country.
- **Gaming characteristics:** device type and game genre.
- **Engagement metrics:** session count and average session length.
- **Spending information:** spending segment, recorded purchase amount, payment method, and purchase-related dates.

**Dataset source:** Mobile Game In-App Purchases Dataset 2025

**License:** CC0 1.0 Universal (Public Domain).

**Dataset author:** Pratyush Puri (Kaggle).

The dataset's collection period, the exact definition of the purchase amount, and the criteria used to assign spending segments have not been verified.

## Data Cleaning and Preparation

The analysis included:

- Checking missing values and duplicate records.
- Confirming unique player identifiers.
- Creating age groups for demographic analysis.
- Preserving missing purchase amounts instead of replacing them with zero.
- Separating total player counts from counts of players with recorded purchase amounts.
- Documenting data limitations before interpreting the results.

There are **136 players with missing purchase-related information: 111 Minnows, 20 Dolphins, and 5 Whales**.

Missing purchase amounts are not assumed to represent zero spending.

## Exploratory Data Analysis

The notebook investigates revenue concentration, age-group performance, game genre differences, geographic revenue distribution, and player engagement.

The analysis uses grouped aggregations, comparisons, summary statistics, and visualizations to answer the defined business questions.

## Key Business Findings

### 1. Revenue Concentration

Whales represent **68 of the 3,024 players**, approximately **2.25%** of the dataset. Of these, 63 have recorded purchase amounts.

The Whale segment accounts for approximately **59.3% of total recorded revenue**.

**Business implication:** Recorded revenue is highly concentrated in a small player segment. Retention initiatives for high-value players may be worth evaluating, although actual retention outcomes cannot be determined from this dataset.

### 2. Revenue by Age Group

Dolphin players aged 25–44 account for **USD 49,734.82**, approximately **51.65%** of recorded Dolphin revenue.

However, this largely reflects the number of players in these age groups. Dolphins aged 45–54 have the highest average recorded purchase amount among Dolphins with known purchase amounts, at **USD 261.35**.

**Business implication:** Marketing decisions should consider both audience size and spending per player rather than relying on total revenue alone.

### 3. Game Genre Performance

Racing, Battle Royale, and Strategy generate the highest recorded revenue among the 15 game genres.

Their Whale player rates are approximately **4.19%, 3.70%, and 4.04%**, compared with approximately **2.25%** across the full dataset.

**Business implication:** These differences warrant further investigation, but they do not establish that game genre causes higher spending.

### 4. Revenue Concentration Across Countries

Several countries have a high share of recorded revenue generated by Whale players.

South Korea, Canada, Italy, Denmark, and Afghanistan show Whale revenue shares ranging from approximately **69% to 80%**.

**Business implication:** Revenue concentration within a small number of players should be considered when evaluating country-level performance.

### 5. Engagement and Spending

Whales average approximately **10.93 sessions**, compared with **10.12 for Dolphins** and **10.04 for Minnows**.

Average session length is approximately **17.93 for Whales**, **20.04 for Dolphins**, and **20.14 for Minnows**.

Within-group variation is substantial relative to these differences.

**Business implication:** The descriptive results do not establish that engagement metrics reliably predict spending or that increasing engagement causes higher revenue.

## Dashboards

### Power BI Dashboard

A business intelligence dashboard was created to present player counts, recorded revenue, segment distribution, game genre performance, and age-group comparisons.

**Project file:** [PowerBI_Dashboard.pbix](PowerBI_Dashboard.pbix)

This file requires Power BI Desktop to open. It cannot be previewed interactively on GitHub.

### AI-Assisted Interactive Dashboard

[▶ Open the Interactive Analytics Dashboard](https://almog1111.github.io/gaming-data-analytics/dashboards/Mobile%20Game%20In-App%20Purchases%20%E2%80%94%20Analytics%20Dashboard.html)

Claude AI was used to generate an additional interactive dashboard based on the original dataset.

The dashboard covers business performance, age groups, game genres, countries, engagement metrics, and data limitations.

It supports interactive filtering and exploratory comparisons.

### On-Demand Device Analysis

A separate natural-language request was used to generate an interactive analysis comparing recorded purchase amounts across device types and spending segments.

The resulting analysis includes interactive charts, a summary table, descriptive statistical comparisons, and business interpretation.

[▶ View the Interactive Device Analysis](https://almog1111.github.io/gaming-data-analytics/dashboards/Device%20Type%20vs%20Recorded%20Spending%20%E2%80%94%20Ad-hoc%20Analysis.html)

The device analysis found higher average recorded spending for iOS players than Android players, but the difference was not statistically conclusive in the reported tests.

AI-generated outputs were reviewed critically rather than treated as automatically correct.

## Project Structure

```text
Gaming-Data-Analytics/
├── data/
│   └── mobile_game_inapp_purchases.csv
├── dashboards/
│   ├── README.md
│   ├── Mobile Game In-App Purchases — Analytics Dashboard.html
│   └── Device Type vs Recorded Spending — Ad-hoc Analysis.html
├── Gaming_Analytics_Final.ipynb
├── PowerBI_Dashboard.pbix
├── mobile_game_inapp_purchases.xlsx
├── README.md
└── requirements.txt
```

## How to Run the Analysis

1. Download or clone the project files.
2. Install Python and Jupyter Notebook.
3. Install the required Python libraries.
4. Ensure the original CSV is located inside the `data` folder.
5. Open `Gaming_Analytics_Final.ipynb`.
6. Restart the notebook kernel and run all cells.

The notebook uses the following relative dataset path:

```text
data/mobile_game_inapp_purchases.csv
```

The Power BI dashboard can be opened separately in Power BI Desktop.

The two HTML dashboards are published through GitHub Pages and can be opened directly using the live links above, without installing additional software.

## Data Limitations

- Some demographic and purchase-related values are missing.
- Missing purchase amounts are not equivalent to zero spending.
- The spending-segment classification criteria are undocumented.
- The dataset's collection period and exact purchase amount definition are unverified.
- The data does not support causal conclusions about spending behavior.
- Country and genre breakdowns may exclude records with missing category information unless those records are explicitly grouped as Unknown.
- AI-assisted statistical outputs require independent verification before being presented as validated results.

## Future Improvements

Future portfolio projects may explore integrating Claude AI into a standalone analytics application.

The goal would be to allow users to ask business questions in natural language and dynamically generate analyses, charts, and dashboards.

This would provide additional experience in AI-assisted analytics, application integration, data validation, and interactive reporting.

## Project Status

Core analysis and dashboard development are complete.

The repository includes the analytical notebook, dataset, Power BI project file, documentation, and two live interactive HTML dashboards published through GitHub Pages.
