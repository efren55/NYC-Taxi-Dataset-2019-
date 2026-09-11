# **NYC Taxi Dataset (2019)**
### Project Overview
This project analyzes New York City’s urban mobility dynamics in 2019 using public NYC Taxi & Limousine Commission (TLC) data. By integrating big data processing with exploratory data analysis, the study evaluates market segmentation, spatial distribution, and rider behaviors across Yellow Taxis, Green Taxis, and High Volume For-Hire Vehicles (FHVHV like Uber and Lyft).

### Project Objective
To evaluate operational efficiency and demand patterns across NYC's transit options in 2019, identifying specific service niches to deliver actionable recommendations for passengers optimizing trip choices and drivers maximizing profitability.

### Flowchart TD
A[NYC Taxi Datasets 2019 - Databricks] --> B[PySpark & Spark SQL: Feature Engineering & Outlier Cleaning]\
B --> C[Cleaned Tables: Yellow, Green & FHVHV]\
C --> D[Export Cleaned Data to CSV]\
D --> E[Jupyter Notebook: Pandas & NumPy Final Cleaning]\
E --> F[LangChain & Google GenAI: Dataset & Column Descriptions]\
F --> G[Univariate, Bivariate & Multivariable EDA: Matplotlib & Seaborn]\
G --> H[Actionable Insights & Conclusions]

## **CONCLUSION**
An analysis of New York’s mobility ecosystem reveals a highly fragmented and specialized market. There is no single "clear winner"; instead, various services have carved out specific niches.\
Yellow Taxis endure as a convenient option for business travel, commanding higher fares for quick, short trips within Manhattan during the workweek. Meanwhile, FHVs (such as Uber and Lyft) have solved the "last-mile" and residential mobility challenge; they dominate weekends and capture demand in the outer boroughs—particularly the Bronx and Brooklyn—outperforming even Green Taxis, whose impact is largely confined to specific border areas like Harlem and western Queens.\
***Actionable Insight:***
- To maximize efficiency, the optimal transport model suggests that users should rely on Yellow Taxis for quick, executive-style trips within Manhattan on weekdays (where the average ride lasts 14 minutes) and turn to FHVs for longer journeys, weekend outings, and travel to or from the outer boroughs. For drivers, the key to profitability lies in positioning themselves in Manhattan during the week (Yellow Taxis) and shifting to residential areas on weekends (FHVs).

## **Insights**
##### A. Market Segmentation: Business vs. Leisure
There is a clear divide in user behavior based on the type of service:
- ***Traditional Taxis (Yellow/Green) = Work-Oriented:*** Demand peaks mid-week (Wednesdays and Thursdays), indicating they are primarily used for business trips, office commutes, and work-related routines.
- ***Apps (FHVHV) = Social and Residential Focus:*** Demand surges on weekends (Saturdays and Sundays). This demonstrates that Uber and Lyft dominate the market for nightlife, social events, and leisure-time mobility.

##### B. Geography and the "Battle" for the Outer Boroughs
The city does not move uniformly; services have carved out distinct territories:
- ***The Manhattan Monopoly:*** Yellow taxis are almost exclusive to Manhattan (concentrating 91% of their trips there), serving as hyper-local transport for the financial and commercial hub.
- ***The Democratization of Transport:*** Apps (FHVs) achieved what traditional taxis could not: connecting the outer boroughs. FHVs have a strong presence in Brooklyn (26%) and dominate the Bronx (11%), outperforming Green Taxis (5%)—which were specifically created to serve those areas.
- ***The Green Niche:*** Green Taxis have found their niche in the areas bordering Manhattan (such as Harlem) and specific parts of Queens (29%) and Brooklyn (27%), acting as a bridge between the city core and the outer areas.

##### C. Trip Economics and User Behavior
Fares and tips reveal how users perceive the value of the service:
- ***Yellow Taxi is a "Premium" service based on convenience:*** It is the most expensive option (9 per mile standard fare vs. 7 for Green Taxis). Its high cost is justified by immediate availability in the city's densest area. Tipping Psychology (The distance effect): Riders tend to be more generous (in percentage terms) on short trips, with the tip proportion decreasing as the trip gets longer. Time of day also plays a role: tips drop during the early morning hours (before 6 AM), yet Green Taxis see an unusual spike in generous tips at midnight.
- ***Card Payment Equity:*** Despite differences in fares, when riders pay by card, the average tip amount standardizes to around $3 per trip for both Yellow and Green Taxis.

##### D. Efficiency and Congestion
- ***Traffic affects everyone equally, though in different areas:*** Yellow Taxis suffer from extreme congestion in Manhattan (speeds of 8.8 to 12.5 mph). However, Green Taxis face even slower traffic (7 to 7.8 mph) on dense local routes in Brooklyn and Queens (e.g., Fort Greene and Jackson Heights), dispelling the myth that only Manhattan suffers from severe traffic flow issues.
- ***Trip Times:*** App-based service (FHV) users experience longer average trip durations (19 minutes) compared to traditional taxis (14 minutes); this makes sense, given that app-based services often handle longer, inter-borough trips.
