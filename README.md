# MyGym-Fitness-Analysis
## Overview
The Fitness Membership Analytics project is a data-driven initiative aimed at uncovering key insights into member engagement, retention, and revenue patterns at MyGym, a fast-growing fitness center chain with multiple locations across California. Using detailed membership, subscription, and service usage data, the project applies data analysis and visualization techniques to identify trends, segment behaviors, and operational inefficiencies. The ultimate goal is to support data-informed decision-making that enhances customer satisfaction, optimizes facility utilization, and drives sustainable growth.

## Project Scope
This project involves a detailed exploration of fitness membership data across MyGym’s multiple locations in California. The analysis focuses on understanding how different subscription types and membership tiers influence retention and revenue. Attention is given to identifying members at risk of churn and the factors that contribute to attrition, alongside evaluating the overall effectiveness of discount types. In addition, the project examines operational aspects such as location performance and resource allocation to highlight areas where efficiency can be improved. All insights are consolidated into interactive dashboards that allow stakeholders to monitor key performance indicators, track trends over time, and make informed decisions that strengthen both customer experience and organizational performance.

## Business Objective: 
The primary objective of this project is to enable MyGym to optimize its membership strategies by:
1.	Identifying high-value member segments and the services that drive loyalty.
2.	Improving retention rates by addressing churn risks and tailoring engagement strategies.
3.	Supporting operational decisions across multiple locations.
4.	Informing pricing and promotional strategies that maximize revenue while maintaining customer satisfaction.
By leveraging data analytics, the project seeks to transform raw membership data into actionable insights that support MyGym’s long-term growth, competitiveness, and member-centric innovation.

## Document Purpose: 
This documentation summarizes the key insights derived from the Fitness Membership Analytics project. This documentation serves as a guide for project stakeholders, providing insights into the project's objectives, data sources, data analysis, and any other relevant information.

## Use case:
The interactive analytics dashboard is intended to serve a variety of stakeholders within MyGym. Potential users and beneficiaries include:
1.	Management Team – The dashboard helps management monitor overall membership performance, assess the financial impact of subscription models, and identify areas where strategic changes can drive growth.
2.	Marketing Department – By analyzing engagement levels, the team can design more targeted campaigns, optimize discount strategies, and attract high-value members.
3.	Operations Team – Insights into location performance enable better allocation of staff and optimization of resources across gyms.
4.	Customer Service & Retention Teams – With access to churn risk indicators and member satisfaction trends, these teams can develop proactive engagement strategies, personalized interventions, and loyalty programs to retain members.
   
## Skills Demonstrated:
●	Data cleaning and preparation

● Data transformation and feature extraction

●	Data validation and quality assurance

●	Dashboard design and visualization in Excel

●	Analytical and critical thinking

●	Communication of data-driven insights

## Data Source:
The dataset used for this project was obtained from an online open-source repository ([Dataset](https://github.com/Rikky101/MyGym-Fitness-Analysis/blob/main/Fitness_Membership_Analytics_Dataset.csv))  for practice purposes. It contains historical membership records from MyGym, covering a diverse range of attributes related to customer demographics, subscription types, and engagement behaviors.
Key variables include member age, membership type (Standard, Premium, etc.), visitation frequency (visits per week, days per week), participation in group lessons, check-in and check-out times, and duration spent in the gym. It also captures additional services such as drink subscriptions, personal training usage, and multi-location access, as well as financial details like discounts applied. Location-based fields (home gym, latitude, longitude) provide geographical context, while timestamps such as join date and last visit date enable retention and churn analysis. 
In total, the dataset comprises 2,001 rows and 26 columns, offering a comprehensive foundation to analyze membership behavior, engagement trends, and operational performance across MyGym facilities. 

## Data Cleaning and Processing: 
The data used in the analysis underwent extensive data cleaning procedures. To guarantee high data accuracy and integrity and to improve the high quality of the dataset, the following steps were carried out:

1.	Identification and Handling of Null Values:
   
    ● Strict procedures were followed to find and deal with any instances of null values on the important columns in each table. In this dataset, null values denote information that is        either missing or insufficient. Incomplete data analysis can produce false results.

    ● The output that results from identifying null values in each table using conditional formatting verifies that the data provided for this study includes all relevant information.         This demonstrates the dataset's completeness and data integrity for this analysis.

2.	Validation and Consistency Checks
   
    ● Checked for duplicate records

    ● It has been verified that there are no duplicate rows in any of the tables used in this study. The data provides different and useful data for the analysis, and each row includes        unique information that ensures the dataset's integrity.

3.	Checking Spelling and Correctness
   
    ● To ensure consistency and dependability, a thorough examination was conducted to verify that all spellings and categorizations were accurate.

    ● Checked for invalid or missing entries in key fields.

    ● Checked for typographical errors. 

4.	Data Standardization and Structuring
   
    ● Ensuring consistency in the format and representation of data, such as standardizing and formatting date formats and text cases.

    ● Reformatted the dataset into a clean, tabular structure optimized for Excel Pivot Tables and dashboard integration. The table was named “mygym”.

    ● Ensured that each record was uniquely identifiable and properly aligned with its attributes.

5.	Data Transformation:
   
     ● Added a new column:
  	
      A new column titled “Membership Status” was created to assess member retention, based on the most recent visit of each member compared to the analysis cut-off date of 31st August        2025. Members who had not visited the gym within the last 60 days before the cut-off date of 31st August. In 2025, they were classified as “Inactive”, while those who had visited        within that period were classified as “Active”. This provides a clear view of how many members are at risk of leaving the gym. This is crucial in designing retention strategies          aimed at converting inactive members back into active users.

      Another column titled “Discount Price” was created to evaluate the impact of promotional offers and member benefits. This column measures the monetary value of discounts applied         to      memberships by calculating the difference between the Adjusted Price (the original or standard price) and the Final Price (the price actually paid by the member after            discounts). This calculation highlights the extent of discounts given across membership types and provides insights into how promotional strategies affect both customer                  acquisition and overall      revenue. 

      Through these steps, the dataset was transformed from raw, inconsistent records into a reliable and structured dataset, ready for analysis and dashboard visualization. This              process      not only improved data quality but also ensured that insights generated from the dashboard are credible and actionable.

## Data Analysis and Visualization:
Dynamic visuals, including column charts, donut charts, and comparative bar charts, were used to create a dashboard to answer the business objectives and convey information intuitively. 

1.	Which membership types are linked to the highest revenue?
    The question refers to the identification of which membership type is the most valuable to MyGym, because members spend more (revenue).
<p align="center">
  <img src="https://github.com/Rikky101/MyGym-Fitness-Analysis/blob/main/Revenue%20by%20Membership%20Type.PNG"
</p>
    
   The chart shows that Premium memberships are the major source of revenue, followed by Standard. Together, these two account for over 70% of MyGym’s income, highlighting their            central importance, followed by Elite and Basic. The analysis suggests that Premium and Standard plans should remain the strategic focus, while Elite and Basic may require re-           evaluation to increase their impact.
    The dominance of the Premium membership type is consistent even when the data is broken down by gender and subscription models. Both male and female members contribute most              significantly to revenue through the Premium plan, confirming its broad appeal across demographics. This consistency suggests that Premium’s value proposition is universally             attractive, cutting across gender differences, and reinforcing its position as the most important revenue driver for MyGym.

2.	Do pricing models (e.g., monthly vs. early bird annual) affect churn or satisfaction?
    This question is asking whether the type of subscription plan that members choose (e.g., monthly, quarterly, annual, or early-bird promotions) has any measurable impact on whether       members on certain plans are more likely to stop visiting or cancel their membership.
    <p align="center">
    <img src="https://github.com/Rikky101/MyGym-Fitness-Analysis/blob/main/Membership%20Status.PNG"
       </p>
    
    The analysis showed that there was no significant overall influence of subscription models on churn rate at MyGym. However, when comparing across individual plans, clear                 differences     emerged. The monthly subscription model recorded the highest churn rate at 63%, suggesting that members on short-term plans are less committed and more likely to         discontinue. This       was followed by the early bird annual model and the quarterly model respectively, both of which also experienced notable churn, but to a lesser degree.
    These findings highlight that while subscription type may not drastically shift the overall churn rate, certain models, particularly monthly memberships, are associated with higher      levels of discontinuation. This insight can guide MyGym to strengthen retention efforts for short-term subscribers, perhaps by offering loyalty incentives or encouraging upgrades to     longer-term plans that foster stronger commitment.

3.	Are some locations performing better than others in terms of engagement or profitability?
    This question examines whether different MyGym locations vary in engagement (how actively members use their memberships) and profitability (how much revenue each branch generates).      In other words, it asks which locations are performing best in keeping members active and which are most financially successful.
 <p align="center">
    <img src="https://github.com/Rikky101/MyGym-Fitness-Analysis/blob/main/Revenue%20by%20Gym%20Location.PNG" 
       </p>
    
   The most successful location by a significant margin is Fresno. With a robust revenue of $8,983, Fresno is a leader in profitability. Cities like Long Beach ($7,402), San Diego          ($7,395), and Sacramento ($7,359) follow, showing similar costs in the upper tier. Oakland, however, showed the lowest revenue. Regular tracking of cost data by the city will help       identify emerging trends and can be applied to cities with lower revenue.

4.	What effect do discount types (promo, student, loyalty) have on final revenue?
    This question is asking whether the different types of discounts offered by MyGym such as promotional discounts, student discounts, or loyalty rewards, have a measurable impact on       the final revenue earned from memberships.
   <p align="center">
     <img src="https://github.com/Rikky101/MyGym-Fitness-Analysis/blob/main/Price%20Analysis.PNG" 
        </p>
      
   Discounts have a clear effect on revenue. The None category shows that sales without any discounts generated the highest final revenue at $33,013. The student discount has the           most significant impact, giving the largest total discount ($3,526) and resulting in the lowest final price. In contrast, the Promo discount has the smallest effect, with the            lowest total discount ($2,101). The Loyalty discount has a moderate impact. 
      The business could explore whether a slightly smaller student discount would still attract the same number of customers, thereby increasing final revenue. Another option is              exploring ways to shift students toward the more profitable Promo or Loyalty options.

5.	Do certain access types (off-peak, all hours, priority) impact visit frequency?
    This question is asking whether the type of gym access a member subscribes to — for example, off-peak (limited hours), all-hours (unrestricted access), or priority (premium,             flexible access)- affects how often members visit the gym.
<p align="center">
   <img src="https://github.com/Rikky101/MyGym-Fitness-Analysis/blob/main/Weekly%20Visits%20by%20Access%20hours.PNG"
      </p>
    
   The data shows that the "All hours" access plan is, by far, the most popular, accounting for a remarkable 2,154 weekly visits. This indicates that members value having unrestricted      access to the facility at any time. Following this, the "Weekdays only" plan also demonstrates strong performance with 1,559 weekly visits, highlighting that many members prefer the     convenience of routine, weekday workouts. Plans with more restrictive or exclusive access attract significantly fewer visits. The "Off-peak only" plan records 1,063 visits, showing      that a segment of customers prefers to avoid peak hours. The least popular plan is "All hours + Priority access," which, despite its premium nature, only garners 571 weekly visits.      This suggests that the value of "priority access" does not translate into high usage for most members.
    This analysis suggests that the business should focus its marketing and resources on the two most popular plans, "All hours" and "Weekdays only," as they are responsible for the         vast majority of member engagement.

[Interact with the dashboard](https://github.com/Rikky101/MyGym-Fitness-Analysis/blob/main/MyGym%20Fitness%20Analysis.xlsx) 

## Recommendation:
1.	Analyze the successful strategies from the Fresno location and apply them to underperforming locations like Oakland to improve profitability.
2.	Focus on the high-value Premium and Standard memberships, as they are the main revenue drivers, and re-evaluate the Elite and Basic plans to increase their impact.
3.	Strengthen retention efforts for members with monthly subscriptions, as they have the highest churn rate (63%), perhaps by offering incentives or encouraging upgrades to longer-term plans.
4.	Reconsider the Student discount as it is the most costly, and explore if a smaller discount would still attract customers or if they can be shifted toward the more profitable Promo or Loyalty options.
5.	Concentrate marketing and resources on the "All hours" and "Weekdays only" access plans, as they are responsible for the vast majority of weekly visits.
   
## Conclusion:
The Fitness Membership Analytics project successfully transformed raw membership data into actionable insights for MyGym. By leveraging data analysis and visualization, the project addressed key business objectives related to member engagement, retention, and revenue.

Thank You for Reading!

Contact me: balogunaryke@gmail.com 
