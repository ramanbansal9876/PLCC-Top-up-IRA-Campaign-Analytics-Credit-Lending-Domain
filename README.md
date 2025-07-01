
# 💡 PLCC Top-up & IRA Campaign Analytics – Credit Lending Domain

## 🔍 Overview
This project aimed to improve the targeting and efficiency of personal loan acquisition through two structured outbound campaigns: the **Top-up Campaign** and the **Interest Rate Advantage (IRA) Campaign**. Together, they targeted over 3.5 lakh customers per month and led to significant improvements in conversion rates and incremental profitability.

## 🧩 Business Objective

- Reduce the inefficiency of blanket telecalling by identifying high-propensity customer segments.
- Design strategic campaigns using timely triggers (e.g., loan maturity or interest rate differentials).
- Improve **conversion rates** and **incremental profitability** through better targeting and segmentation.

## 🧰 Tools & Technologies

- **SQL** – Used throughout all stages: extracting large-scale customer and loan data, applying maturity-based and interest-rate-based filters, and finalizing shortlists with high targeting precision.
- **Microsoft Excel** – Utilized for sharing finalized customer lists with the telecalling team and for version-controlled tracking of campaign performance.
- **Power BI** – Developed interactive dashboards to monitor:
  - Monthly campaign reach and conversion trends.
  - Uplift vs baseline for Top-up and IRA campaigns.
  - Call performance dashboards showing Attempt Intensity (calls per customer from total called batch) and Contact Intensity (calls per customer from total converted batch).
  - Visualization of how many customers from our campaign batch were actually called, how many were connected, and how many remained uncontacted.
  These dashboards provided real-time visibility to business teams and helped optimize ongoing strategy.
- **PowerPoint** – Occasionally used to present campaign performance summaries and long-term trends to internal stakeholders.

## 🧾 Campaign Design & Targeting Criteria

### 1. 📌 Top-up Campaign
- **Goal:** Identify customers who had previously availed personal loans and are likely to need additional credit.
- **Logic:** Select customers whose loans (from own or other institutions) were:
  - Closing within the next 60 days, or
  - Already matured in the past 60 days.
- **Volume:** Targeted ~1.5 lakh customers per month.
- **Action:** Shared filtered customer lists (excluding DNC/NDNC numbers) with the **telecalling team**.
- **Outcome:** Conversion rate improved by **4x** compared to the baseline average.

### 2. 📌 IRA Campaign (Interest Rate Advantage)
- **Goal:** Acquire customers with higher-interest loans from other institutions by offering better repayment terms.
- **Logic:**
  - If the new loan interest rate < existing loan rate → offer directly.
  - If the new loan EMI is lower despite a higher interest rate → offer based on affordability.
  - Used both **interest rate** and **EMI comparison** where available; fallback to EMI when rate was missing.
- **Volume:** Targeted ~2 lakh customers per month.
- **Action:** Prioritized high-opportunity segments for **telecalling outreach**.
- **Outcome:** Conversion rate increased by **11.5x**, significantly boosting monthly acquisitions.

## 📊 Data Preparation & Execution

- Extracted customer data using complex **SQL joins and filters** based on real-time attributes like loan maturity and interest rate.
- Removed customers flagged under **DNC/NDNC** to maintain compliance.
- Used **Excel** to maintain version-controlled campaign sheets and historical tracking of performance.
- Tracked execution using **monthly feedback reports** from the outreach team and refined targeting logic accordingly.

## 🤝 Cross-Team Collaboration

- Worked closely with the **telecalling operations team** to fine-tune targeting logic and validate outcomes.
- Presented insights using **PowerPoint decks** showcasing monthly trends, performance comparisons, and L6M impact.

## 📈 Outcome & Business Impact

| Metric                            | Top-up Campaign         | IRA Campaign              |
|----------------------------------|--------------------------|---------------------------|
| Customers Targeted (Monthly Avg) | ~1.5 lakh                | ~2 lakh                   |
| Conversion Rate Uplift           | ↑ 4x vs baseline         | ↑ 11.5x vs baseline       |
| Incremental Profit (Monthly)     | ₹33 million              | ₹13 million               |

- ✅ **Higher ROI on Outreach** – Avoided targeting the full 30 lakh eligible base by narrowing down to 12–15% high-propensity customers.
- ✅ **Smarter Customer Engagement** – Trigger-based logic helped approach customers with the right offers at the right time.
- ✅ **Sustainable Campaign Strategy** – Monthly refreshes, feedback loops, and compliance screening kept campaigns lean and effective.

## 📌 Key Learnings

- Micro-segmentation using time-bound events and financial logic can drastically improve campaign economics.
- Data + Domain + Delivery = measurable business value.
- A tight feedback loop with execution teams (like telecalling) is essential to measure and iterate effectively.
