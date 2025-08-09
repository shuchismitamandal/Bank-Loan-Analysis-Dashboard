# 📊Bank Loan Analysis Dashboard
A dynamic, interactive Power BI dashboard built to analyze bank loan applications, funding performance, and borrower risk—focusing on loan quality, repayment trends, and borrower characteristics such as purpose, employment, and home ownership. The dataset analysed in this dashboard is financial_loan dataset from Kaggle.

## 🎯Purpose of the Dashboard
Financial institutions often struggle to gain a clear, data-driven understanding of their loan portfolio's performance and associated risks. Without an effective way to track loan volume, repayment behavior, and financial outcomes, decision-makers face challenges in optimizing lending strategies, managing risk exposure, and improving operational efficiency. This project aims to address this gap by developing a Bank Loan Performance & Risk Analysis Dashboard that delivers a comprehensive view of the loan portfolio — enabling stakeholders to make informed, strategic decisions based on real-time insights.   

## 👩‍💻Who is it for?
- **Loan Officers** and **Credit Risk Analysts** assessing loan quality and defaults.
- **Executives** and **Managers** monitoring key performance indicators.
- **Business Stakeholders** looking to optimize lending strategies and customer segmentation.

## ❓Questions Answered

- How has the number of loan applications changed compared to the previous month?
- Which types of loans are most commonly applied for, and which ones receive the most funding?
- Is the bank generating more revenue than the amount it is lending out?
- What is the trend in interest rates and debt-to-income (DTI) ratios over time?
- Which customer segments (based on home ownership or credit grade) are considered low-risk or high-risk?
- Are certain loan purposes or sub-grades more associated with defaults or bad loans?
- How do different states perform in terms of loan repayment and default rates?
- What patterns can be observed in installment amounts, interest rates, and the total recovered amount?


##  Dashboard Insights — A Story Told by Data

### 🏠Summary Page – The Big Picture
*Let’s start with the bird’s eye view.*

This page captures the overall **health and performance of the bank’s lending portfolio**, offering a quick snapshot of how things are moving.

- A total of **38.6K loan applications** have been processed so far, with a **Month-to-Date (MTD)** growth of **4.3K** and a **Month-over-Month (MoM)** increase of **6.9%** — showing consistent loan demand.
  
- The bank has **funded $435.8M** in loans so far, with **$473.1M recovered** — a **positive indicator** of strong collection efforts. The MTD recovery ($58.1M) outpaces funding ($54.0M), which reflects **solid cash inflow**.

- In terms of portfolio quality:
  - **86.2% of loans are categorized as Good Loans**, comprising **33.2K applications**, receiving **$370.2M in funding**, and recovering **$435.8M**.
  - Only **13.8% are Bad Loans**, with **5.3K applications**, funded at **$65.5M**, and only **$37.3M recovered**, indicating a **significant drop-off** in repayment from risky segments.

- The average interest rate stands at **12.0%**, and the average DTI (Debt-to-Income ratio) is **13.3%**, both of which are within a reasonable lending range. This implies **controlled risk** in borrower profiles.

-  From the loan status breakdown:
  - **32K+ loans have been fully paid**, representing a **majority of the portfolio**.
  - **5.3K loans have been charged off**, aligning with the bad loan percentage.
  - Only **~1.1K loans are currently active**, which means **most loans have already matured or been closed**.

 **Overall**, the dashboard shows a **healthy lending portfolio** with a strong share of good loans, **effective recovery**, and **growing demand** — making it a positive signal for stakeholders.
 
 *Here's a visual representation of the Summary page*

![Summary Page](https://github.com/shuchismitamandal/Bank-Loan-Analysis-Dashboard/blob/main/Screenshots/Summary.gif)

### 🧭 Overview Page – Lending Patterns at a Glance  
*Let’s zoom in to understand the customer trends.*

This page dives deeper into how customers are interacting with the bank — who’s borrowing, when they’re borrowing, and for what.

- **Monthly Trend**:  
  Loan applications have shown a **steady upward trend throughout the year**, starting at **2.3K in January** and reaching a peak of **4.3K in December**. This reflects growing demand, possibly due to **seasonal factors or increasing customer confidence**.

- **Term Preference**:  
  A significant **73.2% of applicants (28K)** opted for **60-month loans**, while only **26.8% (10K)** chose the 36-month option — suggesting customers prefer **lower monthly payments** and **longer repayment flexibility**, even if it means paying more interest.

- **By Employment Length**:  
  - Those with **10+ years of experience** made up the **largest segment (8.9K applications)** — indicating that **financially stable and experienced individuals** are the most active borrowers.
  - Applicants with **<1 to 5 years of experience** also make up a decent share (between 3.2K to 4.6K), showing **diverse borrower profiles**.
  - Interestingly, **those with 6 years experience** are the least active (2.2K), which could reflect job switching or career transitions.

- **Loan Purpose**:  
  - **Debt consolidation** is the **top reason**, with **18K applications**, followed by **credit card payoff (5K)** and **others (4K)**.  
    This shows most borrowers are looking to **manage or reduce existing high-interest debt**.
  - Less common but notable purposes include **home improvement (3K)**, **major purchases (2K)**, and **small business needs (2K)** — suggesting some borrowers are also using loans for **value-adding investments**.

- **Home Ownership Status**:  
  - Applicants who **rent (18K)** slightly outnumber those with **mortgages (17K)**.  
    This hints at a large share of **non-homeowners seeking financial support**, possibly due to higher monthly expenses or lack of collateral.
  - Very few applicants own homes outright, indicating **mortgaged and renting individuals form the core of the borrower base**.

✅ **In a nutshell**, this page paints a picture of a growing and diverse borrower base — mostly renters or mortgaged individuals, experienced employees, and debt-conscious citizens — all driving the bank’s lending activity upward.

*Here's a visual representation of the Overview page*

![Overview page](https://github.com/shuchismitamandal/Bank-Loan-Analysis-Dashboard/blob/main/Screenshots/Overview.gif)

### 📋 Details Page – Zooming Into Each Loan  
*Let’s shift from the big picture to the fine print.*

This page gives a **granular view of every single loan** issued — including its purpose, interest rate, installment, repayment, and the borrower’s profile. It's the **backbone of loan-level analysis**, enabling pattern discovery and risk profiling.

#### 🔎 What You Can Explore Here:

- **Loan Purpose**:  
  From **credit cards, small businesses, and education** to **weddings and vacations**, this report spans a variety of borrower needs — giving insights into **which loan types are most common and profitable**.

- **Home Ownership Status**:  
  Borrowers fall into three categories: **OWN, RENT, and MORTGAGE** — useful to evaluate **default likelihood** based on ownership.

- **Credit Grade & Sub-Grade**:  
  - Grades range from **A (low risk)** to **G (high risk)**.  
  - Sub-grades (e.g., A1 to A5, C1 to C5) allow further segmentation.  
  This data is vital for identifying how **interest rates** and **repayment success** vary across creditworthiness levels.

- **Loan Issue Date**:  
  Helps track performance over time and analyze **monthly trends**.

- **Funded Amount vs. Amount Received**:  
  Every record shows how much was **disbursed and recovered**. For example:
  - Loan ID **164346** funded **$500** and recovered **$565**, showing a **13% gain**.
  - Loan ID **311591** (credit card, Grade A1) recovered **$777** on a **$725 loan** — another strong performer.
  
- **Interest Rate & Installment**:  
  - Rates range from **7% to 12%** in this snapshot, based on risk profile.  
  - Monthly installments differ based on term, amount, and interest — some nearing **$32/month**, such as ID **263677**.

*Here's a visual representation of the Details page*

![Details Page](https://github.com/shuchismitamandal/Bank-Loan-Analysis-Dashboard/blob/main/Screenshots/Details.gif)

##  Tech Stack

The dashboard was built using the following tools and technologies:
- Power BI Desktop – Main data visualization platform used for report creation.
- DAX (Data Analysis Expressions) – Used for calculated measures such as MTD, MOM calculations etc.
- Data Modeling – Relationships established among tables (loan_report which is the original dataset and date table which was created manually). 
- File Format – .pbix for development and .png for dashboard previews.

## Data Source

This dashboard was built using the Financial Loan Dataset sourced from Kaggle, comprising a total of 38,576 loan records. The dataset includes detailed information on loan status, borrower demographics, financial metrics, and repayment behavior — providing a solid foundation for in-depth performance and risk analysis.





