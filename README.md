## Bank Customer Churn Analysis | Power BI Dashboard

> Understanding the signals behind customer churn to protect high-value relationships and reduce portfolio risk.
---
##  Business Problem

Customer churn is a critical challenge in the banking sector, directly impacting revenue stability and increasing customer acquisition costs. Identifying at-risk customers and understanding the drivers behind churn is essential for improving retention and customer lifetime value and according to Bain and Company Even a modest 5% improvement in customer retention can drive a disproportionate 25%–95% increase in profitability.

---

## Objective
> Identify High risk customer segments prone to churn
> Analyze behvarioal and financial drivers of churn
> Evaluate customer engagement pattern.
> Enable targeted and data driven retention strategies

---

## Dataset Description
The Dataset includes customer level  information such as:
Demographics(Age,Gender,Geography)
Account Details(Balance,Tenure,Number of products)
Engagement Indicators(Active Status, Credit card usage)
Target variable: **Churn(Exited)**

## Data Model Approach
The dataset follows a **denormalized(flat Table) structure**, Where all attributes are stored in one Single table.

## Key Metrics and KPI's
Churn Rate
Total customers vs Churned customers
Average Balance (churned vs Retained)
Product per customer
Active vs Inactive Customer distribution
**Customer Risk Score(Custom DAX metric)**

---

## Analytical Approach
## Risk  Metric (DAX Based)
A **custome Risk score** was developed using DAX to quantify the likelihood of churn at a customer level.

**Approach:**
> Combined Multiple churn indicators such as:
  - Credit score band
  - Number of products
  - Customer activity status
  - Tenure Patterns
> Each factor contributes to an overall **risk score**, enabling prioritization of customers based on churn likelihood.

**Purpose:**
- Move beyond binary churn (Exited/Retained)
- Create a **continuous risk perspective**
- Help business teams identify and act on **high-risk customers proactively**

## Beyond churn rate
The analysis goes beyond basic churn rate and focuses on  **engagement depth profiling**, including:
- Relationship between number of products and churn likelihood
- Impact of account balance on churn behaviour
- Role of customer activity status in churn
- Segment wise churn patterns across geography and demographics
- Integration of **risk scoring** to priortize customer segments

---

## Key Insights
- **Churn rate stands at ~20%**, indicating a significant erosion of the customer base
- **Customer inactivity is the strongest churn driver**, contributing disproportionately to high-risk segments
- **Germany emerges as the highest churn geography**, with a notable skew among female customers
- **High-balance customers represent concentrated value at risk**, despite lower volume
- **~35% of total customer value (€271M) is concentrated in high-risk segments**, highlighting material revenue exposure

---

## Recommendations
- **Activate dormant customers through targeted re-engagement campagins**, prioritizing high risk inactive segments
- **Deploy geography specifi retention startegies in Germany**, with tailored messaging for high churn cohorts
- **Increase product penetration among single product customers** to strengthen engagement and reduce churn likelihood
- **Priortize high value customers with elevated risk scores** for proactive relationship management
- **Implement early warning using inactivity and risk score signals** to enable pre-emptive intervention

---

## Dashboard features
- Interactive filters (Geography, Gender, Products)
- KPI cards for quick performance tracking
- Visual segmentation of churn drivers
- **Risk-based customer segmentation using custom DAX metric**

---

## Advanced Interactivity (Bookmark-based UX)
- **Bookmark-driven slicer panel**: A collapsible slicer menu implemented as a pop-up for a cleaner dashboard layout
- **Knowledge Pane (Info Button & slicer menu)**: Provides contextual explanations of metrics and visuals for better user understanding and also has Internet linked info which is the website from where info has been implemented in this analysis. Also has the slicer button which opens and close like a menu.
- **Seamless navigation using bookmarks** for a smooth and uncluttered experience

---


## User Experience Design
The dashboard is designed with a focus on **clarity,minimalism and guided analytics**:
- Reduces visual clutter by hiding advanced filters inside a pop up panel
- Enables **self-explanatory insights** through embedded knowledge and info buttons
- Combines **analysis + storytelling + interactivity** for better stakeholder experience

---

## Analysis Demo
> Churn Overview - https://github.com/jeevish/Sample-Banking-Churn-Analysis/blob/main/assets/assets/churn-overview.png
> High-Value Customer Risk - https://github.com/jeevish/Sample-Banking-Churn-Analysis/blob/main/assets/assets/high-value-customer-risk.png
> Behavioral Drivers - https://github.com/jeevish/Sample-Banking-Churn-Analysis/blob/main/assets/assets/segment-drivers-analysis.png
>  Recommendations - https://github.com/jeevish/Sample-Banking-Churn-Analysis/blob/main/assets/assets/recommendation.png
> Interactive slicer - https://github.com/jeevish/Sample-Banking-Churn-Analysis/blob/main/assets/assets/interactive-slicer-menu.png
> Page naviagtion menu -https://github.com/jeevish/Sample-Banking-Churn-Analysis/blob/main/assets/assets/page-navigation-menu.png

---

## Tools & Technologies
- Power BI  
- DAX (Data Analysis Expressions)

---
## How to Use
1. Download the `.pbix` file from this repository  
2. Open using **Power BI Desktop**  
3. Use slicers and filters to explore insights

---

## Conclusion
This project enhances traditional churn analysis by introducing a **DAX-based risk scoring mechanism**, enabling a more proactive and prioritized approach to customer retention. It combines financial, behavioral, and engagement insights to support strategic decision-making.














