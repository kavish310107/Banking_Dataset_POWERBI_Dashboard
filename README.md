# Bank Marketing Analytics Dashboard

An interactive, multi-page Power BI dashboard exploring customer characteristics, marketing contact patterns, and term-deposit subscription outcomes using the Bank Marketing dataset.

## Project Overview

This project uses Power BI to explore the Bank Marketing dataset and examine how customer attributes and marketing contact patterns relate to term-deposit subscriptions.

The dashboard contains two pages:

- **Customer Analysis** — explores age, occupation, education, marital status, loan indicators, and credit-default status.
- **Campaign and Contact Analysis** — explores contact methods, previous campaign contact history, and the number of contacts made during the current campaign.

The detailed dashboard findings and business implications are documented in `Bank_Marketing_Analytics_Dashboard_Report.pdf`.

## Tools and Techniques

- **Power BI Desktop** — dashboard development and interactive reporting
- **Power Query** — data preparation and transformation
- **DAX** — calculated columns, measures, and analytical logic
- **Data visualization** — charts, slicers, and interactive filtering
- **Exploratory Data Analysis (EDA)** — examining patterns across customer and contact attributes

### Data Preparation and Transformation

- Examined the dataset to understand its structure and identify patterns relevant to the dashboard.
- Renamed columns to make them easier to identify and interpret.
- Created age ranges and call-duration ranges from the original columns using DAX.
- Created additional calculated columns and measures to support analysis and dashboard visuals.
- Cleaned date values and converted them into an appropriate date format.
- Used DAX `SWITCH` logic to assign customers to age ranges.
- Combined personal-loan and housing-loan indicators into a derived column using bitwise AND logic.

## Dataset

- **Dataset file:** `bank-full.csv`
- **Source:** [Bank Marketing Dataset on Kaggle](https://www.kaggle.com/datasets/mdnaimislam165436/bank-marketing-dataset-uci)

The dataset contains records from a bank's direct-marketing campaigns. The target outcome indicates whether a client subscribed to a term deposit. Refer to the original dataset page for column definitions and applicable usage terms.

## How to Explore the Dashboard

1. Clone or download this repository.
2. Open the `.pbix` file in Power BI Desktop.
3. Use the slicers and interactive visuals to explore the two dashboard pages.
4. Read `Bank_Marketing_Analytics_Dashboard_Report.pdf` for the EDA process, dashboard findings, and screenshots.

## Interpretation Notes

- The dashboard presents descriptive patterns and does not prove that a customer characteristic or contact strategy causes a subscription.
- Compare subscription counts with conversion rates and group sizes before interpreting a segment as more effective.
- In the dataset, `campaign` represents the number of contacts made to a customer during the current campaign; it is not an identifier for separate campaigns.
- Previous campaign contact history and current-campaign contact frequency are different variables.
- Findings can change depending on report filters, data-cleaning choices, and the dataset version.
- The meaning of any derived loan indicator depends on the exact DAX expression used and should be documented clearly in the Power BI model.

## Future Improvements

- Add clearly defined subscription-rate measures for customer and contact segments.
- Display segment size alongside conversion rates.
- Add explicit KPI definitions and filter context.
- Compare contact methods using both contact volume and subscription rate.
- Further investigate contact-frequency patterns while accounting for relevant customer characteristics.
- Document the calculated columns, measures, and transformation rules.

## Skills Demonstrated

**Power BI · DAX · Power Query · Data Cleaning · Exploratory Data Analysis · Data Visualization · Business Analytics**
