# ZOOMRIDES-ANALYSIS(SQL)

## Project Overview
This project delivers a structured analysis of ride-hailing sales performance for ZoomRides, a multi-city transportation platform operating across Lagos, Abuja, Port Harcourt, Accra, Nairobi, and Kampala, offering both car and bike ride services similar to Uber and Bolt.
Using SQL, the project queries and examines key business questions around revenue, ride volume, city-level performance, and demand pattern translating raw transactional data into clear, actionable insights.

---

## Data Overview & Cleaning Process

The database consists of three tables ; Customers, Drivers, and Trips , with the Trips table being the largest and most central to the analysis.
The raw data required cleaning before analysis. This involved removing duplicate records, trimming unnecessary whitespace, and correcting spelling inconsistencies to ensure uniformity across all fields. Once cleaned, the data was reliable and ready to accurately answer the 
targeted business questions.

---

## Impact of Data Cleaning 
-Before cleaning total number of trips recorded 300, after cleaning number of trips recorded 298.
-Before cleaning Lagos recorded 88, after cleaning it recorded 93
-Before cleaning Abuja recorded 36 trips, after cleaning it remained same but recorded as second to highest number of trips
-Before cleaning Accra recorded 33, after cleaning it recorded 37 now ranking second to the highest
-Before cleaning Nairobi recorded 27,after cleaning it recorded 32
-Before cleaning Port Harcourt recorded 26,after cleaning it recorded 31
-Before cleaning Kampala recorded 17,after cleaning it recorded 19

---

## BUSINESS QUESTIONS ANSWERED
1. Which city earns the most money?
2. Which month do people ride the most?
3. Which type of vehicle earns the most money?
4. Which customer(s) didn't book a trip?
5. Which customer(s) spent more on trips?

---
## Tools Used
1. MySQL
2. One compiler

---
## Key Insights
1.Lagos recorded the highest overall demand, leading all cities in total revenue and number of trips completed, while also ranking second for average fare.
2.Economy vehicles recorded the highest overall demand, leading all categories in total revenue and number of trips completed.
3.December 2025 recorded the highest overall demand, leading all months in total revenue and number of trips completed.
4.4 Customers never booked a trip, investigation needs to be carried out to know why. It could be their trip was cancelled and they got offended or no knowledge on how to book a trip.
5.The highest number of completed trips booked by a customer was 21,with a total revenue of NGN 38,950.

# MESSAGE TO MANAGER
## Recommended City for Investment: Lagos
Based on the analysis, Lagos is the strongest candidate for investment, with 93 total trips — nearly 3× the volume of the second-highest city (Accra, 37 trips) — and total revenue of NGN 218,890, approximately 38% of overall platform revenue. Its average fare of NGN 2,405 remains competitive and consistent, though some null fare values are yet to be recovered and warrant further investigation.
A monthly trend breakdown further supports this recommendation. Lagos generated NGN 90,910 in the first half (July – December 2025) and NGN 127,980 in the second half (January – June 2026), reflecting 41% revenue growth between both periods. While month-to-month fluctuations were observed, the underlying growth trajectory is clear.

## Data Quality Issues Identified
Two data integrity problems were found and corrected during the cleaning phase. Inconsistent city names and spacing — entries such as Nairobbi, Kampla, PH, and Port-Harcourt caused trip counts and revenue to be fragmented across multiple rows, producing incorrect totals and misleading city rankings. After standardisation, Accra correctly moved into second place behind Lagos.

## Limitations & Open Questions
While the data supports Lagos as the top-performing city by revenue and volume, revenue alone does not confirm profitability. Before a final investment decision is made, the following questions should be addressed:

1.What are the operating costs per city (driver incentives, logistics, support overhead)?
2.Does Lagos face heavier competition, requiring discounts that compress margins?
3.How does profit per trip compare across cities when costs are factored in?

Notably, Accra holds the highest average fare at ₦2,807, which could indicate stronger per-trip profitability if its cost base is lower. A complete cost dataset would allow for a reliable profit-per-trip comparison and a more definitive recommendation.

## CONCLUSION & RECOMMENDATION
Lagos is the clear investment priority. It leads all cities with 93 trips and NGN 218,890 in revenue — 38% of total platform revenue — and grew 41% in the second half of the period, signaling strong and rising demand.
Data quality issues were identified and resolved. Misspelled city names had fragmented trip records across multiple entries, understating each city’s true performance. After cleaning, Accra emerged as the second-highest city with 37 trips and the highest average fare of NGN2,807.
However, before committing to Lagos, I recommend gathering:
-Cost data per city to assess actual profitability
-Reasons behind monthly revenue fluctuations
-Clarity on unrecovered null fare values

Revenue leadership does not guarantee the highest margins. Accra’s superior average fare makes it worth monitoring closely once cost data becomes available
Occurrence of null values in the fare,this needs to be investigated and recorded.
