# PALMORA GROUP HR ANALYSIS

## TABLE OF CONTENTS

- [PROJECT OVERVIEW](#project-overview)
- [DATA SOURCE](#data-source)
- [TOOL](#tool)
- [DATA CLEANING AND PREPARATION](#data-cleaning-and-preparation)
- [EXPLORATORY DATA ANALYSIS](#exploratory-data-analysis)
- [INSIGHTS AND KEY FINDINGS](#insights-and-key-findings)
- [SUMMARY OF KEY GENDER INSIGHT FOR MANAGEMENT](#summary-of-key-gender-insight-for-management)
- [VISUALIZATION](#visualization)
- [RECOMMENDATIONS](#recommendations)
- [CONCLUSION](conclusion)
- [DAX QUERIES](dax-queries)

### PROJECT OVERVIEW

This data analysis project explores gender inequality within Palmora Group, a manufacturing company operating across three regions in Nigeria. Following recent media coverage branding the organization as “Palmora, the Manufacturing Patriarchy”, the company faces increasing scrutiny over its internal HR practices. By examining various aspects of the HR dataset, this project aims to uncover patterns, highlight disparities, and provide data-driven recommendations to address gender imbalance and improve equity within the workforce.

### DATA SOURCE

This analysis is based on two primary datasets:
- Palmoria Group emp-data.csv – Contains detailed employee information such as gender, department, region, salary, and ratings.
- Palmoria Group Bonus Rules.xlsx – Outlines the bonus allocation rules based on employee ratings and department.

It contains detailed information on the company’s workforce, including employee profiles and salary data. These datasets were merged to support an in-depth analysis of gender distribution, salary structure, bonus allocation, and gender-related disparities within Palmoria Group.

### TOOL
The analysis was conducted using Power BI [Download Here](https://www.microsoft.com/en-us/download/details.aspx?id=58494)
  - leveraging the Power Query Editor for efficient data cleaning, transformation, and merging.
  - This enabled seamless integration of the datasets and preparation of the data for visualization and insight generation.

### DATA CLEANING AND PREPARATION

In the initial phase of the project, the following steps were carried out:
1. Extracted, transformed, and loaded the employee dataset.
2. Extracted and loaded the bonus mapping data separately.
3. Merged both datasets to create a unified view for analysis.
4. Performed data cleaning and formatting, including:
    1. Handling missing or inconsistent values
    2. Adding calculated columns for bonus and total compensation
    3. Changing data types to ensure proper analysis in Power BI

### EXPLORATORY DATA ANALYSIS

The Exploratory Data Analysis phase focused on uncovering key insights from the HR dataset to better understand gender dynamics, salary structure, and regulatory compliance across Palmoria Group’s three regions. The following focus areas were explored:
- Bonus Calculation
    - Calculated the bonus amount payable to each employee based on their department and performance rating.
    - Computed the total compensation (salary plus bonus) for individual employees.
- Regional and Company-wide Salary Insights
    - Determined the total payroll amount per region and for the entire organization.
- Gender Distribution Analysis
    - Examined the gender breakdown across the company, with further analysis by region and department.
- Performance Ratings by Gender
    - Analyzed employee performance ratings to identify any patterns or disparities by gender.
- Salary Structure and Gender Pay Gap
    - Assessed the overall salary distribution to detect gender pay gaps.
    - Identified specific regions and departments where the pay gap is most significant and may require management attention.
- Compliance with Minimum Salary Regulation
    - Evaluated whether Palmoria meets the newly adopted regulation requiring a minimum salary of $90,000 for manufacturing employees.
    - Analyzed employee salary distribution in $10,000 bands (e.g., $10,000–$20,000, $20,000–$30,000, etc.)
    - Visualized salary bands across different regions to provide a comprehensive view of pay distribution.
 
### INSIGHTS AND KEY FINDINGS

#### 1. Overall Gender Distribution:
    - Total Employees: 946 (100%)
    - Males: 465 (49.15%)
    - Females: 441 (46.6%) 

**Insight**: The gender split is nearly equal, which suggests good company-wide representation.

#### 2. Overall Average Salary:
    - Male: 77,000
    - Female: 74,595

Pay Gap Metric: 96.81%
This means Female employee earns only 96.81 cents for every $1 men earn. A 3.2% gender pay gap which means female employee earn 3.2% less than male employees on average 

**Insight**: This is close to equal pay but not quite there yet, this gap grows larger at department and regional levels.

#### 3. Pay Gap by Department

From the table of Average Salary by Gender and Department:

|Department|Female Salary|Male Salary|
|----------|-------------|-----------|
|Sales|72306.06|74134.45|
|Business Development|76940.51|84488.89|
|Engineering|77944.18|79028.61|
|Legal|70183.26|74148.18|
|Marketing|82219.77|76549.30|
|Training|80427.31|76888.16|

**Insight**:
- Business Development, Legal, and Engineering show the most significant gaps against women.
- Marketing and Training are the only departments where females earn more.

#### 4. Pay Gap by Region

|Region|FemaleSalary|Male Salary|
|------|------------|-----------|
|Abuja|72970.59|75530.26|
|Kaduna|74571.93|77083.71|
|Lagos|76624.75|78772.97|

**Insight**:
- In every region, male employees earn more than female employees.
- Gaps are consistent and suggest systemic patterns.

#### 5. Salary Band Compliance
    - Employees earning < $90,000: 618
    - Employees earning ≥ $90,000: 328

From gender bar visuals:
- More men than women are in the above $90k bands.
- More women are clustered in the $50k–$80k bands.

**Insight**:
- This shows a glass ceiling effect: fewer women in top-earning brackets.
- Might indicate fewer leadership roles or promotions among female employees.

#### 6. Departmental Representation

From the Gender Distribution by Department chart:
- HR, Services, Support, Legal: More female employees
- Engineering, Product Management, Sales, R&D: More male employees

**Insight**:
- Women are more represented in support and admin roles.
- Underrepresentation in technical and revenue-driving roles (often higher paying).

#### 7. Performance Ratings
- Males received slightly more "Average" and "Good" ratings.
- Both genders are similarly represented across rating categories.

**Insight**: There is no strong gender bias in ratings, but this should be analyzed deeper if ratings affect bonuses or promotions.

### VISUALIZATION

![Palmora final Table](https://github.com/user-attachments/assets/02ea7c82-c7ed-4713-8f9b-55470cf5c48e)


![palmora model view](https://github.com/user-attachments/assets/547439cd-ab4d-44b3-96c5-4cd1bd140e2d)


![palmora Dashboard 1](https://github.com/user-attachments/assets/09bcbd3d-8640-4d1b-811b-cead116218aa)


![Palmora Dashboard 2](https://github.com/user-attachments/assets/f3d9ab60-547d-4a29-95b6-d3af47f35e5b)


### SUMMARY OF KEY GENDER INSIGHT FOR MANAGEMENT
1. Workforce Balance	Near equal male and female counts company-wide.
2. Gender Pay Gap	Exists company-wide (3.2%) and larger in key departments.
3. Departmental Disparity	Women underrepresented in technical and leadership-heavy departments.
4. Regional Pay Gap	Men earn more in all regions (Abuja, Kaduna, Lagos).
5. Salary Band Distribution	Fewer women in the Above or 90,000 compliance band.
6. Salary Gaps in departments like Business Development and Legal have biggest pay gaps favoring men.
7. Exception department like Marketing & Training show women earning more.

### RECOMMENDATIONS
- Conduct Salary Audits: Address pay disparities, especially in departments like Business Development and Legal.
- Promote Female Representation in High-Paying Roles: Encourage women into technical and leadership roles through targeted recruitment and mentorship.
- Standardize Compensation Across Regions: Ensure fair pay for women across Abuja, Kaduna, and Lagos.
- Support Career Growth for Women: Introduce leadership programs and promotion pathways to help more women reach top salary bands.
- Train Managers on Gender Equity: Implement bias training and hold leaders accountable with gender equity scorecards.
- Establish an Equity Monitoring Team: Create a task force to track progress and drive continuous improvement.

### CONCLUSION
Palmora demonstrates commendable gender balance in overall workforce numbers, but there are still notable disparities which remains in compensation, departmental roles, and salary progression. To strengthen its commitment to equity, the company should prioritize closing gender pay gaps, increasing female representation in high impact roles, and promoting a culture of inclusion. These actions will not only ensure compliance but also reinforce Palmora’s position as a progressive and equitable employer.

### DAX QUERIES
```dax
Gender Pay Gap = DIVIDE(CALCULATE(AVERAGE('palmoria HR DATA'[Salary with Bonus]), 'palmoria HR DATA'[Gender] = "Female"), CALCULATE(AVERAGE('palmoria HR DATA'[Salary with Bonus]), 'palmoria HR DATA'[Gender] = "Male") ) * 100
```








