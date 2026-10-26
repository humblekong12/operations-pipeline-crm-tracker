# operations-pipeline-crm-tracker
A data-driven CRM database simulation demonstrating pipeline tracking, real-time status updates, data schema logging, and exception workflows modeled after modern Applicant Tracking Systems (ATS).




## Project 2: Operations & Customer Pipeline CRM Tracker
**Objective:** Build a data-driven tracking pipeline to manage operations, log data, and handle time-sensitive customer requests. This layout structurally mirrors workflows found in standard Applicant Tracking Systems (ATS) like Greenhouse.

### 1. Data Schema & Pipeline Structure
The pipeline tracks orders from initial intake to final verification across the following structured stages:

| Stage | Action Items | Data Captured |
| :--- | :--- | :--- |
| **1. Intake** | Order receipt, basic verification | Customer Name, Phone, Item Details |
| **2. Production** | Fulfillment coordination | Completion ETA, Priority Level |
| **3. Quality Check** | Weight, packaging, and order accuracy | Notes on anomalies or custom specs |
| **4. Logistics & Delivery** | Time-slot assignment, routing | Delivery Window, Driver Assignment |
| **5. Completed** | Follow-up, archival, and log locking | Feedback Rating, Privacy Check |

### 2. Incident & Exception Handling Workflows
* **Missed Deliveries / Delays:** Move record to a high-priority "Exception Queue." Flag for an automated follow-up call within 15 minutes.
* **Customer Communication Logging:** All interactions (calls, text confirmations) are appended with timestamps and a concise summary to keep internal teams aligned.
* **Data Privacy Protection:** Personal identifiable information (PII) like phone numbers and delivery addresses are kept confidential, visible only to authorized fulfillment staff.

