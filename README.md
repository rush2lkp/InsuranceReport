INSURANCE RISK & CLAIMS ANALYSIS
DOMAIN DOCUMENT
This dataset contains detailed information about car insurance policyholders, their vehicles, and their claim history. Each record represents an individual customer with demographic details such as birthdate, gender, marital status, education level, household income, and parental status. These attributes provide a strong basis for understanding customer profiles and how personal characteristics may influence driving behaviour and insurance risk.
The dataset also captures rich details about the insured vehicle, including car make, model, colour, year of manufacture, and usage type (personal, commercial, or commuting). Combined with the coverage zone, this information helps in assessing environmental and vehicle-related risk factors. For example, an older car used for commercial purposes in an urban area may carry a different risk profile compared to a new personal car in a rural zone.
On the financial and claims side, the dataset includes claim amount (total cost of claims filed), claim frequency (number of claims filed), and household income. These fields are critical in evaluating customer value and risk. High-frequency claimants may signal higher risk, while high claim amounts could indicate severe accidents or expensive repairs. The Kids Driving field adds another dimension, reflecting household driving behavior, since households with multiple young drivers are typically considered riskier by insurers.
Overall, this dataset offers a comprehensive view of customers, vehicles, and claims. It can be used to build Power BI dashboards for claims analysis, customer segmentation, risk profiling, and premium optimization. Insights derived from the data can help insurance companies design fairer pricing models, identify high-risk segments, detect potential fraud, and improve customer targeting strategies.

1. ID
Definition: A unique identifier assigned to each policyholder or insurance record.
Type: Numeric or text (Primary Key).
Details:
Ensures each policy/customer record is unique.
Not used directly in analysis but essential for data integrity, relationships, and avoiding duplicates.
Business Use: Helps track individual policyholders across multiple datasets (e.g., linking claims, payments, or renewals).

2. Birthdate
Definition: Date of birth of the policyholder.
Type: Date.
Details:
Used to calculate the Age of the policyholder.
Age is a strong factor in insurance risk assessment (younger drivers may have more accidents, older drivers may have slower reflexes).
Business Use:
Segment customers into age groups (e.g., <25, 25–40, 40–60, 60+).
Age-based pricing of premiums and risk profiling.

3. Car Color
Definition: The exterior color of the insured car.
Type: Categorical (text).
Details:
Although color doesn’t directly affect risk, it can influence car visibility, theft probability, and customer preferences.
Business Use:
Explore patterns (e.g., some studies suggest red cars might be involved in more speeding cases).
Insights for fraud detection (unusual color-claim patterns).

4. Car Make
Definition: The manufacturer/brand of the car (e.g., Toyota, Ford, BMW).
Type: Categorical.
Details:
Different makes have varying repair costs and accident likelihood.
Business Use:
Analyze claims by car brand.
Identify which brands have higher claim frequency (riskier) vs lower claims (safer).
Useful for underwriting and premium adjustments.

5. Car Model
Definition: Specific model of the car (e.g., Toyota Corolla, BMW X5).
Type: Categorical.
Details:
Provides deeper granularity beyond car make.
Claim risk can vary significantly between models of the same make.
Business Use:
Compare claims for luxury vs economy models.
Useful for loss ratio analysis by vehicle type.

6. Car Use
Definition: The primary purpose of the car (e.g., Personal, Commercial, Commute).
Type: Categorical.
Details:
Commercial and commuting cars usually have higher claim rates due to greater exposure (more time on the road).
Business Use:
Pricing policies differently for personal vs commercial use.
Risk profiling based on usage patterns.

7. Car Year
Definition: The manufacturing year of the car.
Type: Numeric.
Details:
Helps calculate Car Age = Current Year – Car Year.
Older cars may break down more often or have lower resale/repair costs.
Business Use:
Assess claim likelihood by vehicle age.
Create segments like New (<3 years), Mid-age (3–10 years), Old (>10 years).



8. Coverage Zone
Definition: The geographic risk area where the policyholder resides/uses the car (e.g., Zone A, Urban, Rural).
Type: Categorical.
Details:
Location impacts accident probability, theft risk, and repair costs.
Urban areas → higher claim frequency, rural areas → fewer accidents but possibly more severe damage.
Business Use:
Compare performance across regions.
Useful for mapping dashboards in Power BI.

9. Education
Definition: The highest education level attained by the policyholder (e.g., High School, Graduate, Postgraduate).
Type: Categorical.
Details:
Education level often correlates with income and risk behavior.
Business Use:
Check claim frequency by education group.
Insights for marketing campaigns and segmentation.

10. Gender
Definition: Gender of the policyholder (Male, Female, Other).
Type: Categorical.
Details:
Gender differences in claim patterns may exist.
Business Use:
Risk analysis by gender group.
Demographic breakdowns in dashboards.

11. Marital Status
Definition: Marital status of the policyholder (Single, Married, Divorced, etc.).
Type: Categorical.
Details:
Married people are often seen as more stable, potentially lower risk.
Business Use:
Compare claims between singles vs married customers.
Factor in pricing and risk adjustment.

12. Parent
Definition: Whether the policyholder has children (Yes/No).
Type: Boolean / Categorical.
Details:
Parents may drive differently compared to non-parents.
Business Use:
Segment claims and policies by parent status.
Combine with Kids Driving for more detailed household analysis.

13. Claim Amt
Definition: Total monetary value of claims filed by the policyholder.
Type: Numeric (currency).
Details:
A critical measure of insurance losses.
Business Use:
Used to calculate total losses, average claim amount, and claim ratios.
Identify high-cost claims for fraud detection.

14. Claim Freq
Definition: The number of claims filed by the policyholder.
Type: Numeric (integer).
Details:
Frequency of claims indicates risk behavior.
Business Use:
KPI for customer risk assessment.
Combined with Claim Amt → identifies whether risk is due to high frequency or high severity.

15. Household Income
Definition: Annual income of the policyholder’s household.
Type: Numeric.
Details:
Income level affects affordability of premiums and vehicle type.
Business Use:
Segment customers into income bands.
Compare claim patterns across income groups.
Target marketing/policy offers (e.g., premium insurance for high-income households).

16. Kids Driving
Definition: Number of kids in the household who are licensed drivers.
Type: Numeric (integer).
Details:
Values (1, 2, 3…) indicate number of kids driving.
More kids driving generally = higher accident probability.
Business Use:
Analyze claims by number of kids driving.
Group into categories (e.g., None, 1 Kid, 2 Kids, 3+ Kids).
Helps insurers estimate family household risk.


![Dashboard_Preview](https://github.com/rush2lkp/Insurance_Report/blob/main/Power_ScreenShot.png) 

![Dashboard_Preview](https://github.com/rush2lkp/Insurance_Report/blob/main/Power_ScreenShot.png)

















