## Title: COHORT, RETENTION ANALYSIS
# Author: Oluwadara Olamide 

## Project Title
Weekly Subscription Retention & Churn Analysis (Cohort-Based)

## Task Description

I received a follow-up task from the Product Manager to analyse how subscription churn behaves from a **weekly retention perspective**. The Product Manager highlighted that monthly retention views can be slow to reveal behavioural patterns and may result in missing critical insights.
To address this, I applied **cohort analysis**, which allows user retention and churn to be tracked over time based on when subscribers started their subscriptions.

The objective of this task was to:
* Identify how many users started their subscription in a given week.
* Track how many of those users remained active over the following **six weeks**.
* Present weekly retention cohorts from **Week 0 to Week 6**.
* Perform the analysis as of **7 February 2021**.

The analysis was carried out using the `turing_data_analytics.subscriptions` table in **Google BigQuery**, with further analysis and visualisation completed in **Microsoft Excel**.

## Tools Used

* **Google BigQuery** – for data extraction and transformation
* **Microsoft Excel** – for cohort analysis and visualisation

## Project Files

* **`cohort.sql`**
  Contains the SQL query used to extract and prepare weekly cohort retention data from BigQuery.

* **` COHORT, RETENTION ANALYSIS.xlsx`**
  Excel workbook containing the analysis and visual outputs. The file includes three sheets:

  1. **Sheet 2** – Cleaned and structured cohort data extracted from BigQuery
  2. **Cohort Analysis** – Weekly retention cohort table (Week 0 to Week 6)
  3. **Visualisations** – Charts illustrating retention and churn trends over time

## Analytical Approach

1. Identified each subscriber’s **cohort week** based on their subscription start date.
2. Calculated weekly retention by tracking whether subscribers remained active in subsequent weeks.
3. Normalised retention values to allow comparison across cohorts.
4. Visualised cohort behaviour to identify churn and retention patterns clearly.

## Key Findings
**Insights**

1. The churn rate experienced a **significant spike during the festive period**, followed by a noticeable decline in the weeks afterwards.
2. The **20 December 2020 cohort** recorded the **lowest churn rate**, indicating strong early retention among users who subscribed during that period.

## Key Concepts Addressed

* **User Retention**
  The ability of a business to keep users active over a defined period of time.

* **Churn Rate**
  The percentage of users who discontinue their subscription during a specific time window.

* **Relationship Between Retention and Churn**
  Retention and churn are inversely related — as retention increases, churn decreases.

* **Negative Churn**
  Occurs when revenue gained from existing users (e.g. upgrades or reactivations) exceeds revenue lost from churned users.

* **User Retention Cohorts**
  Groups of users segmented by a shared characteristic, in this case, the week they started their subscription, enabling behavioural comparison over time.

## Conclusion

This cohort-based weekly retention analysis provides faster and more actionable insights compared to monthly reporting. By identifying churn patterns early, stakeholders can respond proactively with targeted retention strategies, particularly around high-risk periods such as festive seasons.
