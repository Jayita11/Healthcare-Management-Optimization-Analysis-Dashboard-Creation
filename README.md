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

#### Financial & Insurance Dashboard

- The total billing amount reached **$1.40B** across all hospitals, with significant growth in 2020 before seeing a dip in 2024. However, the data only reflects the numbers up to May 2024, so there is potential for an increase by the end of the year. This downward trend highlights the dynamic nature of healthcare demands and the impact of external factors on revenue, possibly due to operational adjustments post-pandemic.
- The average billing per patient is **$25.54K**, with minor variations between insurance providers. **Medicare** leads with an average billing of **$25.63K**, while **UnitedHealthcare** follows closely at **$25.41K**, suggesting consistent pricing strategies across the board.
- Patients in the **30-39 age** group contributed the highest total billing (**$208.17M**), followed by those aged **40-49** with **$204.83M**, indicating that middle-aged patients are a key demographic for healthcare spending. This also suggests that individuals in these age groups may be more prone to health issues, necessitating higher healthcare expenditures.
- Admissions are evenly distributed among **Elective (33.70%)**, **Urgent (33.42%)**, and **Emergency (32.88%)** cases, demonstrating that all patient care types are significant contributors to overall billing.

![Finance Dashboard](https://github.com/user-attachments/assets/ab543d23-8c41-45c8-a0d5-2c25fed833e9)

#### Patient Insight Dashboard

- **Low-risk patients** contribute the most to total billing (**$467M**), while **high-risk patients** account for **$158M**. This indicates that routine monitoring and care for low-risk patients is a critical revenue stream, as they may require frequent checkups and follow-up appointments, even if their conditions are not life-threatening.
- The number of patient admissions peaked in **2020** at **3,818**, followed by a gradual decline. The significant decrease in 2024 can be attributed to external factors like healthcare policies or global events. However, as the data only includes records up to May 2024, there is potential for admission rates to increase by the end of the year.
- The gender distribution is nearly balanced, with **50.02% male** and **49.98% female** patients, indicating equitable access to healthcare services across genders.
- Patients aged **50-59 years** and **30-39 years** have the highest admission rates, representing critical age groups for hospital resource planning and patient care management. These groups may require urgent care more frequently, highlighting the need for hospitals to prioritize resource availability for these patients.

![Patient Dashboard](https://github.com/user-attachments/assets/a0c933f1-387f-4a00-8231-086e0f1a9c9e)

#### Hospital & Doctor Dashboard

- **LLC Smith** hospital leads in overall billing, contributing **$423,591**, along with the highest elective admissions. **Ltd Smith** hospital follows closely behind, showcasing their efficiency and revenue generation capabilities. Some refund amounts were also noted, indicating billing adjustments, possibly due to insurance claims or patient refunds.
- **Michael Smith** is the top-performing doctor, generating **$201K** in billings for high-risk patients. **John Smith** and **Robert Smith** significantly contribute with **$275K** and **$186K**, respectively. Interestingly, low-risk patients who require discharge and follow-up appointments contribute a substantial portion of the total billing. This suggests that even though these patients are at lower risk, maintaining contact and follow-up with their doctors generates a considerable revenue stream.
- The average length of stay varies between doctors, with **Jessica Johnson** having the shortest average stay of **19 days** for elective cases, while **William Johnson** averages **26 days**, highlighting differences in case complexity and doctor efficiency. Elective cases tend to have shorter average stays compared to emergency and urgent cases, which underscores the need for hospitals to adopt tailored resource management strategies based on admission type.

![Hospital   Doctor Dashboard](https://github.com/user-attachments/assets/b43f48d1-dfd3-4bbf-9b60-13af6765ccad)

#### Common Medical Conditions and Medications SQL Analysis 

- Arthritis ranks highest in terms of medication demand, with **9,218 prescriptions** recorded, emphasizing the significant pharmaceutical needs for managing chronic pain.
  
- Diabetes and Hypertension follow as the next most common conditions, both requiring consistent medication management to prevent long-term complications. These conditions have a high impact on hospital resources and medication supply.

- Aspirin is the most frequently prescribed medication for multiple conditions such as **Arthritis**, **Asthma**, and **Cancer**, highlighting its importance across treatment categories.

- Paracetamol and Ibuprofen are widely prescribed for pain and inflammation, while Penicillin is commonly used for managing infections in **Obesity** and **Diabetes** patients. Additionally, **Lipitor** is essential for managing chronic diseases like **Diabetes** and **Obesity**, indicating its critical role in long-term treatment plans.

#### Universal Blood Donors and Receivers

- There are **6,804 universal blood donors (O-)**, which are crucial for emergency situations, as O- blood can be safely transfused to any patient. This makes it a vital resource for hospitals, especially during shortages or emergencies.

- **6,882 patients** are classified as universal receivers (AB+), which allows them to receive blood from any donor. This flexibility in transfusion provides hospitals with greater options for managing blood supply during critical times.

- The near-equal distribution of **O- donors** and **AB+ receivers** ensures a balanced potential for blood supply and demand, helping hospitals mitigate shortages and optimize blood bank strategies.

- A stored procedure, **Blood_Matcher**, was created to prioritize matching donors and receivers within the same hospital for faster and more efficient transfusions. For instance, **Bobby Harvey**, a 79-year-old AB+ patient, was successfully matched with multiple O- donors from different hospitals, ensuring a timely and compatible transfusion at **Lester-Rogers hospital**.

## Recommendations:

- With the majority of patients aged **30-49 years** contributing significantly to hospital revenue, **target preventive care initiatives** and resource allocation for this age group to enhance patient outcomes and reduce long-term healthcare costs.

- **Prioritize preventive care** for high-billing conditions like **obesity** and **diabetes**, focusing on early intervention and management to reduce the need for costly treatments later on.

- Despite the balance of **O- universal donors** and **AB+ universal receivers**, **enhance blood bank management** by optimizing cross-hospital donor-matching systems to ensure timely and efficient transfusions during emergencies.

- **Recognize and incentivize top-performing doctors** such as **Michael Smith** and **John Smith**, who generate substantial revenue through high-risk and follow-up patients. Consider offering incentives and expanding their services to increase patient retention and maximize revenue.

- **Investigate the decline in total billing in 2024** and address operational inefficiencies or external factors that may have impacted hospital revenue. Adjust financial strategies for the remainder of the year to help recapture potential lost revenue.

- To manage high medication demand for chronic conditions like **Arthritis**, **Diabetes**, and **Hypertension**, **optimize pharmacy inventory** by ensuring a steady supply of key medications, such as **Aspirin**, **Paracetamol**, and **Lipitor**, while minimizing costs through bulk purchasing or supplier negotiations.

- **Leverage historical data** to optimize bed allocation, balancing resources between short- and long-term stays. This will ensure that hospitals can handle both urgent and elective admissions efficiently without overextending resources.

- **Strengthen relationships with key insurance providers** like **Cigna** and **Medicare** to ensure steady patient admissions and maintain financial stability. Collaborating with these insurers can help streamline billing practices and reduce discrepancies.

- **Maintain an optimal inventory of high-demand medications** like **Aspirin** and **Paracetamol** to ensure consistent pharmaceutical management. Regular audits of inventory can minimize shortages and prevent overstocking, while supplier negotiations can help manage costs.


