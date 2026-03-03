# Fraud-Transaction-Analysis
This project analyzes transactional data to identify fraud patterns, monitor fraud rate trends, and support risk-based decision-making.

**Business Objectives**

- Monitor total fraud exposure

- Track fraud rate (%) over time

- Identify high-risk transaction types

- Analyze fraud distribution by location

- Evaluate device usage patterns

- Support data-driven fraud mitigation strategies

**Key KPIs**

Total Transaction Amount: 118.6M

Total Transactions: 39.6K

Total Fraud Cases: 1.9K

Fraud Rate: 4.9%

Average Transaction Amount: 3.0K

**Dashboard Features**

**Fraud Summary View**



- Fraudulent transactions by transaction type

- Fraud trend analysis over time

- Fraud vs non-fraud distribution

- Location-based fraud analysis

- Interactive filters (Transaction Type, Payment Method, Status)

**User & Device Analysis**

- Transaction count by device used

- Fraud by previous fraud history

- Fraud by payment method

- Detailed transaction-level log

- Drill-down capability for deeper investigation

**Key Insights**

- Fraud rate stands at approximately 4.9%, indicating measurable risk exposure.

- Certain transaction types show significantly higher fraud concentration.

- Fraud distribution varies by location, suggesting potential geographic risk clusters.

- Device usage patterns highlight possible device-specific fraud behavior.

- Users with previous fraud history demonstrate higher likelihood of repeat fraud.

**Tools & Technologies**

- Looker Studio – Dashboard development & visualization

- Google Sheets / CSV (Data Source)

- Calculated Fields – KPI & fraud metric computation

 **Sample Calculated Fields (Looker Studio)**
Total Transactions = COUNT(Transaction ID)

Total Fraud = COUNT(CASE WHEN Status = "Fraud" THEN Transaction ID END)

Fraud Rate (%) = Total Fraud / Total Transactions

Total Transaction Amount = SUM(Transaction Amount)

**Data Structure**

The dashboard is built on a structured transactional dataset containing:

- Transaction ID

- User ID

- Location

- Device Used

- Transaction Type

- Payment Method

- Status (Fraud / Not Fraud)

- Transaction Amount

- Timestamp

**Business Value**

This dashboard enables:

- Faster fraud detection

- Improved monitoring of high-risk segments

- Better resource allocation for investigation teams

- Strategic fraud prevention planning

It can be adapted for fintech, digital banking, payment platforms, and e-commerce businesses.

**Dashboard Preview**

(Insert your dashboard screenshots here)

(Insert your dashboard screenshots here)

**Recommendations**

Based on the analysis, the following actions are recommended:

**Implement Risk-Based Monitoring**
- Prioritize monitoring for high-risk transaction types and locations with elevated fraud rates.

**Device-Level Risk Flagging**
- Introduce enhanced verification or step-up authentication for devices associated with repeated fraud activity.

**Customer Risk Scoring**
Develop a simple risk scoring framework incorporating:

- Previous fraud history

- Transaction frequency

- Device usage patterns

- Location risk exposure

**Time-Based Fraud Monitoring**
- Investigate peak fraud time windows and introduce targeted monitoring during high-risk periods.

**Payment Method Controls**
- Apply stricter verification measures for payment methods with higher fraud concentration.

**Continuous KPI Tracking**
- Maintain ongoing monitoring of fraud rate trends to quickly detect spikes or unusual patterns.
