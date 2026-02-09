# Service Reminder Optimization System

## Background

In 2024, the Customer Payment Unit Service (CPUS) achievement at the Tangerang branch reached only **92% of the annual target**. Analysis showed that the main constraint was not operational effort, but the **quality and quantity of the customer database** used for service reminders.

From an average of **2,000 customer records per month**, the funnel performance showed the following results:

- **90%** Connected  
- **60%** Contacted  
- **25%** Booking On Call (BOC)  
- **26%** Came After Invited (CAI)

With this funnel performance, CAI contributed only **74% of the monthly CPUS target** (700 units). As a result, the branch relied heavily on **walk-in customers and additional marketing activities** to achieve the target.

Two improvement opportunities were identified:

1. Improving funnel quality through database validation, optimized calling time strategies, and stronger persuasive skills.
2. Expanding database potential by analyzing customer service behavior based on **service timing** and **service type**.

This project focuses on the **second approach**, leveraging **behavior-based data enrichment** to sustainably increase CAI contribution to CPUS achievement.

---

## Objectives

- Increase CAI contribution toward CPUS achievement  
- Classify customers based on **service timing behavior** (Late, Early, Punctual)  
- Segment customers based on **service type behavior** (Periodic Maintenance, General Repair, Oil Change)  
- Enrich the customer database to enable more targeted and effective reminders  
- Reduce dependency on walk-in customers  

---

## Tools & Technologies

- **BigQuery** – Processing and analyzing customer data into actionable datasets  
- **AppSheet** – Operational application for MRA & SA to access and utilize potential data  
- **Looker Studio** – Monitoring dashboard for real-time CPUS performance tracking  

---

## Workflow & Usage

### Flow 1: Data Processing (BigQuery)

Raw data is transformed into structured and actionable insights.

- **Data Collection**: Aggregating all Work Orders from 2020–2024  
- **Cleansing & Enrichment**: Ensuring data accuracy and enriching customer attributes  
- **Service Categorization**: Classifying services into:
  - PM (Preventive Maintenance)
  - GR (General Repair)
  - GO (Oil Change)
- **Habit Analysis**: Identifying customer service behavior patterns  
- **Final Classification**: Consolidating data into a Final Potential Classification and storing it in the Potential Database  

🔗 **BigQuery Scripts**  
https://github.com/gangga211298/Service-Reminder-Optimization/blame/main/BigQuery_Script

---

### Flow 2: Operational Execution (AppSheet)

The stage where customer engagement is executed.

- **Assignment**: Potential data is distributed to MRA & SA based on category  
- **Platform Access**: Data is accessed through the AppSheet application  
- **Engagement**: Service reminders are delivered via phone or WhatsApp  
- **Logging**: Interaction outcomes are recorded directly in the application  
- **Synchronization**: Field updates are automatically synced to the dashboard  

🔗 **Application Access**  
https://www.appsheet.com/start/02ddea69-fdd2-460f-b3c0-4a59487d35dc
<img width="1280" height="720" alt="Presentation1" src="https://github.com/user-attachments/assets/75941462-aaac-4b5f-89b4-2f8a2de4fb9a" />

---

### Flow 3: Monitoring & Evaluation (Looker Studio)

Performance visibility and decision support for management.

- **Real-time Sync**: Operational data is synchronized automatically  
- **Managerial Review**: Service Managers monitor:
  - Connected & Contacted Rate  
  - BOC, CAI, and CPUS Achievement  
- **Decision Making**: Strategic actions based on performance insights  

🔗 **Dashboard Access**  
https://lookerstudio.google.com/reporting/7bb40189-df21-45b6-bbe6-3ed44a7fc568
![NKIM_-_Dashboard_Monitoring_UDA_page-0001](https://github.com/user-attachments/assets/31f3fe0d-5e92-4bab-83bb-f8f8b91e7df6)

![NKIM_-_Dashboard_Monitoring_UDA_page-0002](https://github.com/user-attachments/assets/5b75e0e7-461e-440c-b7da-5c3be31f0cfa)

---
<img width="406" height="571" alt="GGR" src="https://github.com/user-attachments/assets/bcb0933c-9114-4dc4-8284-ddb955f587d2" />

---

## Results & Insights

### Results

- A structured **Potential Database** was built based on customer service history and behavior  
- Reminder activities became more targeted and prioritized  
- End-to-end integration achieved across BigQuery, AppSheet, and Looker Studio  
- Real-time monitoring enabled better control of Connected, Contacted, BOC, CAI, and CPUS metrics  

### Insights

- Database quality and structure have a greater impact than data volume alone  
- Behavior-based segmentation improves conversion prioritization  
- System integration reduces reliance on walk-in customers  
- Real-time data supports faster and fact-based decision making  

---

## Key Learnings

- **Data quality comes first**  
  Well-structured and reliable data delivers better outcomes than simply increasing data volume.

- **Behavior-based segmentation is more effective**  
  Customer segmentation based on service habits provides more actionable insights.

- **End-to-end integration matters**  
  Seamless integration accelerates execution and evaluation.

- **Data must be usable, not only accurate**  
  Field users must easily access and understand data for adoption.

- **Real-time visibility drives better decisions**  
  Live monitoring enables faster and more informed managerial decisions.
