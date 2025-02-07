### **Overview of the Dashboard**

This report analyzes customer churn trends and identifies key factors driving customer attrition. The objective is to enhance retention strategies and reduce revenue loss.

### **Data collection:**

As a part of my virtual internship with PwC Switzerland, I was provided with a dataset to complete this project.

[view dataset here]
[02 Churn-Dataset.xlsx](https://github.com/user-attachments/files/18709307/02.Churn-Dataset.xlsx)


### **Data  Preparation and transformation:**

- **Data transformation** was performed in Power Query, and the dataset was loaded into Microsoft Power BI Desktop for modeling.
- The dataset consists of **23 columns and 7,043 rows** under the table name **Customer Churn Dataset**.
- **Data Cleaning steps**:
    few steps include
    - Standardizing response values in the certain columns.
    - Added a new column **Loyalty**
    
    ```
    loyalty check = SWITCH(TRUE(),
    'Churn Data'[tenure]<=12,"1 Year",
    'Churn Data'[tenure]<=24,"2 Years",
    'Churn Data'[tenure]<=36,"3 Years",
    'Churn Data'[tenure]<=48,"4 Years",
    'Churn Data'[tenure]<=60,"5 Years",
    'Churn Data'[tenure]<=72,"6 Years"
    )
    ```
    
    - Removed unnecessary rows and columns.
    - Ensured each column has the correct data type and ready for analysis.
### **Key Findings**

### **1.Customer Overview**

- **Total Customers:** 7,043
- **Retention Rate:** 73.46% (5,174 retained customers)
- **Churn Rate:** 26.54% (1,869 churned customers)
- **Revenue Impact:**
    - Total Revenue: **$456.12K**
    - Revenue Lost Due to Churn: **$139.13K (30.50%)**
    
     ![CHURN HOMEPAGE](https://github.com/user-attachments/assets/89b08b27-f765-42bb-9896-cf42815cf0fa)
     ![CHURN PAGE1](https://github.com/user-attachments/assets/32668ea0-903c-4188-8dba-247636810693)


### **2.Churn Insights**

- **Demographics & Behavior:**
    - Senior Citizens (41.68%) have a higher churn rate.
    - Customers with No Dependents (31.28%) and No Partners (32.96%) are more likely to churn.
- **Service & Contract Analysis:**
    - Month-to-Month Contracts (42.71%) contribute to the highest churn.
    - Fiber Optic Internet Users (41.89%) churn more than DSL or other services.
    - Electronic Check Users (45.29%) have the highest churn.
    - Customers with No Tech Support (41.64%) are at higher risk.
- **Billing & Charges Impact:**
    - Paperless Billing Users (33.57%) show higher churn.
    - Customers with Total Charges above $85 experience a 13.21% higher churn rate.
    - First-Year Customers (47.44%) are most likely to churn.
      ![CHURN PAGE2](https://github.com/user-attachments/assets/498bdde6-0113-403e-8c8a-fa5fca204f48)

      ![CHURN PAGE3](https://github.com/user-attachments/assets/53ec039b-0183-404b-8a7b-787d39bb4b94)
      ![CHURN PAGE4](https://github.com/user-attachments/assets/dd306912-4685-47d2-90df-e72f8bfc7fa2)


### **3. Key Churn Drivers**

1. **Contract Type (42.71%)** – Month-to-month plans lead to higher churn.
2. **Internet Service (41.89%)** – Fiber optic users have increased churn.
3. **Payment Method (45.29%)** – Electronic check users are at higher risk.
4. **Loyalty Check (47.44%)** – First-year customers have the highest churn rate.
5. **Lack of Additional Services** – Online backup, security, and streaming services impact churn.

    ![CHURN PAGE5](https://github.com/user-attachments/assets/0edb4a70-9eb4-4607-8c37-52a107682b18)

### **Recommendations to Reduce Churn**

 **Improve Retention Strategies:**

- Offer **longer-term contracts** (discounted annual plans) to mitigate churn from month-to-month contracts.
- Provide **exclusive perks or discounts** for loyal customers.

 **Enhance Customer Engagement & Support:**

- Encourage **tech support enrollment** for at-risk customers.
- Offer **better service for Fiber Optic users** to reduce dissatisfaction.

 **Optimize Pricing & Payment Options:**

- Address **high churn among electronic check users** by incentivizing auto-pay or credit card payments.
- Monitor and **adjust high total charges** exceeding $85 to improve retention.

 **Targeted Retention Campaigns:**

- Special **loyalty programs** for first-year customers.
- Promotions for **customers without additional services** to encourage adoption.

### **Conclusion**

Reducing churn requires a multi-faceted approach focusing on contract optimization, service enhancement, pricing adjustments, and customer engagement. Implementing these strategies will help in minimizing revenue loss and improving overall customer satisfaction.
