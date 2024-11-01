# Adventure-Works-Report
Power BI project analyzes

## The Situation: 
Suppose **AdventureWorks** Company hired you as **Business Intelligence Analyst**.
AdventureWords is a manufacturing company that produces cycling equipment and accessories.

## The Brief:
The management team needs a way to **track KPIs** (sales, revenue, profit, returns), **compare regional performance, analyze product-level treands, & identify high-value customers.**

They gave you a **folder of raw data csv files**, which contain information about transactions, returns, products, customers, and sales territories.
[Click Here](https://github.com/SudesnaDebnath/Adventure-Works-Report/tree/main/Adventure-Works-Raw-Data)

## The Objective:


###### 1. Connect and Transform the Raw Data
Useing **Query Editing Tools** in **PowerBI **Transform the raw data in the back-end, and 
organized them before loading data into front-end of PowerBI 

###### 2. Build a Relational Data Model
Build Relationship between **Fact Tables** and **Dimension Tables** using **Primary/Foreign Keys** 
**Primary Key(PK):** They uniquely identify each row of the table, and relate to **foreign keys** in **fact tables**

**Foreign Key(FK):** They contain multiple instances of each value, and relate to **primary keys** in **dimension tables**

**Note:**
We create connection between **Primary key and Foreign key** directly.(Use Star Schemas)
If we want to build connection between same type keys then connection will be indirectly.(Use Snowflake Schemas)

**Rules:**
1. Building a normalized model.
2. Oraganized dimension(lookup) tables above fact(data) tables
3. Avoid complex relationships unless absolutely necessary
4. Hide fields from report view to prevent invalid filter context

###### 3. Create Calculated Columns & Measures with DAX
1. Use calculted columns for filtering.
2. Use measures for aggreating values.
3. Use Expllicit measures.(Explicit measures can be referenced anywheere, and nested within ohter measures)
4. Use fully-qualified column references in measures(This makes DAX more readable, and differentiates column references from measure references)
5. Move column calculations **"upstream"** when possible
6. Minimize the use of "**expensive"** iterator functions

###### 4. Design an Interactive DashBoard to Visualize the Data
Use Matrix, Tables, KPI, Cards, Text Cards, Gauges, Bar Charts, Line Charts, Donut Charts, Slicers,... etc.
Filtering, formating, and design to get better view for End User.
Use Drill up/down/through filters.
Also use Interractions to customize how filters applied to one visual impact other visuals on the page
Use Bookmarks capture the current state of a page, and allow users to return to that state using report actions.
and also create Mobile Layout
Create a navigation bar which can interactive with other pages, and also use [icons](https://github.com/SudesnaDebnath/Adventure-Works-Report/tree/main/Adventure-Works-Images)
And so on.

**Target:**
Easy to understand for End-User

#### Conclusion:
A well-designed dashboard should serve a distinct purpose for a distinct audience, use clear and effective metrics and visuals, and provide a simple, intutitive user experience.

[Check Dashboard](https://github.com/SudesnaDebnath/Adventure-Works-Report/blob/main/AdventureWorks%20Report.pbix)
