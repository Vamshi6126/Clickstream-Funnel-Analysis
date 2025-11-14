# Week 1 – Progress Update
**Dataset Used**: E-Commerce Clickstream & Transaction Data (Kaggle ZIP)
This week I mainly focused on understanding the new dataset I downloaded and planning the work needed before building the Power BI dashboard.
## 1. Understanding the Project
The goal of the project is to find out where users drop off in the e-commerce sales funnel.  
The funnel we are focusing on is:
- Homepage  
- Product Page  
- Add to Cart  
- Checkout  
- Purchase
- his analysis will help the business identify issues such as device-related drop-offs or campaign performance problems.
## 2. Understanding the Dataset
After extracting the ZIP file, I checked the CSV files included.  
The dataset contains clickstream events (user interactions) and transactions (orders).
Some key fields I noticed:
- event_time  
- event_type (page view, cart add, purchase, etc.)  
- product_id  
- user_id  
- session_id  
- price / order_value  
These fields will help build the funnel steps.
## 3. Data Cleaning Requirements (Planned)
While checking the dataset, I identified several things that need cleaning:
- Missing values in some columns  
- Duplicate rows in events  
- Different formats of event names (example: “add_to_cart”, “AddToCart”, etc.)  
- Wrong data types for timestamps and numeric fields  
- Inconsistent device information  
- Some events without proper session IDs
- I will handle all of this in Power Query during Week 2.
## 4. Session Logic
The dataset has session IDs, but some may be missing or repeated.  
If required, I will recreate session IDs using the 30-minute inactivity rule to maintain accuracy in the funnel.
## 5. Data Model Planning
I planned the star schema that I will use in Power BI:
**Fact Tables**
- fWebEvents  
- fOrders  
**Dimension Tables**
- dDate  
- dProduct  
- dUser  
- dDevice  
- dSession  
This structure will help build clean relationships between the tables.
## 6. Dashboard Layout Planning
I also sketched how the dashboard pages will look:
**Page 1 – Funnel**
- Funnel chart for all stages  
- KPIs: Sessions, Orders, Conversion Rate, AOV  
- Filters: Device, Traffic Source, Date  
**Page 2 – Traffic & Campaign**
- Sales by traffic source  
- Conversion by source  
- CPA (if cost data is available)  
**Page 3 – Drop-off Details**
- Sessions that abandoned the cart  
- Last page visited  
- Device/browser level filtering
## Week 1 Summary
This week, I completed the foundation work:
- Understood the project goal  
- Analyzed the new dataset  
- Prepared a cleaning checklist  
- Planned session logic  
- Designed the star schema  
- Planned dashboard structure  

Next week, I will begin loading the dataset into Power BI, clean it using Power Query, build the data model, and start developing the funnel page.
