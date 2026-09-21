
# Insurance-Dashboard (Prism Insurance Pvt. Ltd.)

### Dashboard Link :https://suraj-shukla45.github.io/Insurance-Data-Analysis-Power-BI-/

## Problem Statement

This dashboard helps an insurance company (Prism Insurance Pvt. Ltd.) understand its policy, premium and claims performance in one place. It shows how much premium is collected, how much coverage is provided and how much is being claimed, so the company can quickly see which policy types and customer age groups drive the most claims.

It also shows how many policies are active vs. inactive and how claims are distributed across Rejected, Settled and Pending status. With this, the company can identify areas to work on, such as reducing pending claims, understanding the high number of rejected claims and improving policy retention.

Since total claim amount (16.91M) is much higher than the total premium amount (5.98M), the company must closely monitor claim costs and pricing of high-claim policy types like Travel and Health.

Also, since around 42% of policies are inactive, they should work on renewal and retention strategies.

## Tools Used

- Power BI Desktop
- Power BI Service
- DAX

## Steps followed

- Step 1 : Load the insurance dataset into Power BI Desktop.
- Step 2 : Open Power Query Editor and check "column distribution", "column quality" and "column profile" (based on entire dataset) to find errors and empty values.
- Step 3 : Clean the data and fix data types where required.
- Step 4 : Apply a theme from the View tab in report view.
- Step 5 : Add a text box with the company name **PRISM INSURANCE PVT.LTD.**
- Step 6 : Add slicers (filters) for **Policy Number**, **ClaimNumber**, **CustomerID** and **Gender** (Female / Male).
- Step 7 : Add three card visuals for **Premium Amount**, **Coverage Amount** and **Claim Amount**.
- Step 8 : Add a bar chart showing **Premium Amount by PolicyType**.
- Step 9 : Add a donut chart showing **Active / Inactive** policies.
- Step 10 : Add a ribbon chart showing **Count of ClaimStatus by ClaimStatus** (Rejected, Settled, Pending).
- Step 11 : Add a line chart showing **Sum of ClaimAmount by Age Group** (Adult, Elder, Young Adult).
- Step 12 : Add a matrix showing claim amount by **PolicyType** (rows) and **ClaimStatus** (columns: Pending, Rejected, Settled) with totals.
- Step 13 : Format visuals (rounded cards, borders, shadows, titles) for a clean look.
- Step 14 : Publish the report to Power BI Service.

<!-- Add your DAX measures / calculated columns here, for example: -->
<!-- Premium Amount = SUM(<table>[PremiumAmount]) -->
<!-- Claim Amount = SUM(<table>[ClaimAmount]) -->

# Snapshot of Dashboard

<img width="1584" height="859" alt="Image" src="https://github.com/user-attachments/assets/99252ad7-5d57-472b-8f2a-7828eb801497" />
# Insights

A single page report was created on Power BI Desktop and then published to Power BI Service.

Following inferences can be drawn from the dashboard;

### [1] Key Numbers

- Total Premium Amount = 5.98M
- Total Coverage Amount = 600.55M
- Total Claim Amount = 16.91M

Claim amount is around 2.8 times the premium amount collected.

### [2] Premium Amount by Policy Type

1. Travel - 2.5M
2. Health - 1.2M
3. Auto - 1.0M
4. Life - 0.7M
5. Home - 0.6M

        thus, Travel policies bring the highest premium (around 42% of total premium).

### [3] Active vs Inactive Policies

- Active policies = 5.82K (58.13 %)
- Inactive policies = 4.19K (41.87 %)

        thus, a good number of policies are inactive, so renewal / retention needs attention.

### [4] Claim Status

- Rejected claims = 4.4K
- Settled claims = 3.4K
- Pending claims = 2.3K

        thus, the number of rejected claims is the highest, followed by settled and pending claims.

### [5] Claim Amount by Age Group

- Adult - 8.8M
- Elder - 6.4M
- Young Adult - 1.7M

        thus, Adults contribute the highest claim amount, and Young Adults the lowest.

### [6] Claim Amount by Policy Type and Claim Status

| Policy Type | Pending | Rejected | Settled | Total |
|---|---|---|---|---|
| Auto | 10,58,322.67 | 0.00 | 16,66,024.45 | 27,24,347.1 |
| Health | 14,34,634.01 | 0.00 | 19,97,685.01 | 34,32,319.0 |
| Home | 6,24,844.16 | 0.00 | 9,70,918.49 | 15,95,762.6 |
| Life | 8,75,430.45 | 0.00 | 11,87,574.15 | 20,63,004.6 |
| Travel | 28,14,011.25 | 0.00 | 42,82,858.09 | 70,96,869.3 |
| **Total** | **68,07,242.53** | **0.00** | **1,01,05,060.19** | **1,69,12,302.7** |

        thus, Travel has the highest total claim amount, followed by Health and Auto.
        Settled claims (about 60 %) are higher than Pending claims (about 40 %) in amount.
        Rejected claims carry 0 claim amount.

Values will change if different slicers (Policy Number, ClaimNumber, CustomerID, Gender) are applied.
