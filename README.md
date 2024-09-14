# Healthcare Management Optimization Analysis & Dashboard Creation

## Project Background

The **Healthcare Management Optimization** project leverages data from 2019 to May 2024 across multiple hospitals to provide critical insights into hospital operations, patient care, and financial management. This project aims to assist hospital administrators and healthcare providers in making data-driven decisions to improve efficiency, optimize resources, and enhance patient care.

With the rising demand for urgent, elective, and emergency care, hospitals face challenges in optimizing patient stay durations, managing billing practices, and ensuring efficient allocation of resources such as blood supply and medical staff. The dataset used in this project provides a comprehensive view of hospital operations, including patient demographics, hospital stay durations, medical conditions, insurance billing, and doctor performance across various facilities.

### Key insights and recommendations are provided across the following areas:

- **Patient Stay Duration**: Evaluation of patient stay lengths across hospitals, aimed at improving capacity management for both short- and long-term care.
- **Billing Practices by Insurance Providers**: Analysis of billing discrepancies and trends across different insurance providers, helping to identify areas for cost optimization.
- **Blood Supply Management**: Insights into universal blood donor and receiver distributions to ensure timely and efficient transfusions.
- **Doctor Performance**: Evaluation of doctors based on the number of patients treated and their associated billing, offering insights into workload and revenue contribution.
- **Medication Trends**: An analysis of the most commonly prescribed medications for various medical conditions, guiding pharmacy inventory management.

An interactive Tableau dashboard accompanies this project to provide a dynamic and visual exploration of the findings. 

Excel was used to inspect, clean, and prepare the data for analysis, ensuring accurate and actionable insights.

The SQL queries regarding various business questions and data preparation for the Tableau dashboard can be found [here](#).

By harnessing this data, healthcare providers can address key operational challenges, reduce costs, and improve the overall quality of patient care.

### Dataset

This project utilizes a Kaggle dataset of patient records from multiple hospitals, highlighting key metrics such as hospital stay duration, billing amounts, insurance providers, and medical conditions. 

![Pink Minimalist Skincare Brand Comparison Chart Table Graph](https://github.com/user-attachments/assets/fc34944f-7c55-4d34-bced-1568391f0fc8)

## Executive Summary

### Overview of Findings

This analysis provides key insights into the operational and financial performance of the healthcare system from 2019 to May 2024. Three main findings emerge:

1. **Steady Financial Growth**: The total billing amount reached **$1.40B** across all hospitals, with significant growth in 2022 before seeing a dip in 2024, reflecting the dynamic nature of healthcare demands.
2. **Balanced Patient Admissions**: Admissions for **Elective**, **Emergency**, and **Urgent** cases contributed almost equally to the total billing, suggesting a well-rounded approach to patient care.
3. **Top Performers in Hospitals and Doctors**: Certain hospitals and doctors consistently contribute to the highest billings, such as **LLC Smith** hospital and **Michael Smith**, who generated **$201K** in billings, highlighting potential areas for optimizing operations and recognizing key contributors.


### Insights Deep Dive

#### Financial & Insurance Dashboard

- **Total Billing Trends**: The total billing amount reached **$1.40B** across all hospitals, with significant growth in 2020 before seeing a dip in 2024. However, the data only reflects the numbers up to May 2024, so there is potential for an increase by the end of the year. This downward trend highlights the dynamic nature of healthcare demands and the impact of external factors on revenue, possibly due to operational adjustments post-pandemic.
- **Insurance Provider Billing**: The average billing per patient is **$25.54K**, with minor variations between insurance providers. **Medicare** leads with an average billing of **$25.63K**, while **UnitedHealthcare** follows closely at **$25.41K**, suggesting consistent pricing strategies across the board.
- **Age-Based Billing**: Patients in the **30-39 age** group contributed the highest total billing (**$208.17M**), followed by those aged **40-49** with **$204.83M**, indicating that middle-aged patients are a key demographic for healthcare spending. This also suggests that individuals in these age groups may be more prone to health issues, necessitating higher healthcare expenditures.
- **Admission Types Contribution**: Admissions are evenly distributed among **Elective (33.70%)**, **Urgent (33.42%)**, and **Emergency (32.88%)** cases, demonstrating that all patient care types are significant contributors to overall billing.

#### Patient Insight Dashboard

- **Risk Category Distribution**: **Low-risk patients** contribute the most to total billing (**$467M**), while **high-risk patients** account for **$158M**. This indicates that routine monitoring and care for low-risk patients is a critical revenue stream, as they may require frequent checkups and follow-up appointments, even if their conditions are not life-threatening.
- **Admission Trends**: The number of patient admissions peaked in **2020** at **3,818**, followed by a gradual decline. The significant decrease in 2024 can be attributed to external factors like healthcare policies or global events. However, as the data only includes records up to May 2024, there is potential for admission rates to increase by the end of the year.
- **Gender Distribution**: The gender distribution is nearly balanced, with **50.02% male** and **49.98% female** patients, indicating equitable access to healthcare services across genders.
- **Age Group Admissions**: Patients aged **50-59 years** and **30-39 years** have the highest admission rates, representing critical age groups for hospital resource planning and patient care management. These groups may require urgent care more frequently, highlighting the need for hospitals to prioritize resource availability for these patients.

#### Hospital & Doctor Dashboard

- **Top Hospital Performance**: **LLC Smith** hospital leads in overall billing, contributing **$423,591**, along with the highest elective admissions. **Ltd Smith** hospital follows closely behind, showcasing their efficiency and revenue generation capabilities. Some refund amounts were also noted, indicating billing adjustments, possibly due to insurance claims or patient refunds.
- **Doctor Billing Performance**: **Michael Smith** is the top-performing doctor, generating **$201K** in billings for high-risk patients. **John Smith** and **Robert Smith** significantly contribute with **$275K** and **$186K**, respectively. Interestingly, low-risk patients who require discharge and follow-up appointments contribute a substantial portion of the total billing. This suggests that even though these patients are at lower risk, maintaining contact and follow-up with their doctors generates a considerable revenue stream.
- **Length of Stay by Doctor**: The average length of stay varies between doctors, with **Jessica Johnson** having the shortest average stay of **19 days** for elective cases, while **William Johnson** averages **26 days**, highlighting differences in case complexity and doctor efficiency. Elective cases tend to have shorter average stays compared to emergency and urgent cases, which underscores the need for hospitals to adopt tailored resource management strategies based on admission type.

---

This detailed breakdown of findings offers actionable insights for optimizing financial performance, patient care, and hospital resource allocation across the healthcare system.
