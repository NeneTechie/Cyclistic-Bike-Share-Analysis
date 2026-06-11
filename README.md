Cyclistic-Bike-Share-Analysis
Data analysis case study using Python (pandas, matplotlib, seaborn) to uncover behavioral differences between Cyclistic bike-share members and casual riders — Google Data Analytics Capstone Project.

Project Overview

This project is a data analysis case study completed as part of the 
Google Data Analytics Professional Certificate.

I analysed historical bike trip data from Cyclistic, a fictional 
bike-share company in Chicago, to answer the following business question:

How do annual members and casual riders use Cyclistic bikes differently?

The insights from this analysis were used to develop 3 data-driven 
marketing recommendations designed to convert casual riders into 
annual members — increasing company revenue and long-term growth.

Business Context

Company: Cyclistic Bike-Share — Chicago, USA  
Stakeholder: Lily Moreno, Director of Marketing  
My Role: Junior Data Analyst  
Framework: Ask → Prepare → Process → Analyse → Share → Act

Cyclistic operates 5,800+ bicycles across 600+ docking stations
in Chicago. The company offers three pricing plans:
- Single-ride passes
- Full-day passes
- Annual memberships

The finance team confirmed that annual members are significantly more 
profitable than casual riders. The goal is to understand the behavioral 
difference between both groups and use those insights to drive conversions.


❓ Business Question

> How do annual members and casual riders use Cyclistic bikes differently?
>Datasets used
> ivvy_Trips_2019_Q1.csv | Jan – Mar 2019 | ~365,000 | Motivate International Inc. |
| Divvy_Trips_2020_Q1.csv | Jan – Mar 2020 | ~426,000 | Motivate International Inc. |

Data Source:[Divvy Trip Data](https://divvy-tripdata.s3.amazonaws.com/index.html)  
License: Public data made available by Motivate International Inc.  
Privacy: No personally identifiable information is included.

Tools used
Python | Primary analysis tool |
| pandas | Data loading, cleaning and analysis |
| matplotlib | Creating charts and visualisations |
| seaborn | Chart styling and formatting |
| JupyterLab | Interactive coding environment |
| PowerPoint | Presentation of findings |

Data Cleaning Steps

Before analysis, the following cleaning steps were performed:

1. Renamed 2019 columns to match 2020 column names
2. Selected only the 8 relevant columns from both datasets
3. Merged both datasets into one unified DataFrame using `pd.concat()`
4. Converted `started_at` and `ended_at` from text to datetime format
5. Standardised rider labels — replaced `Subscriber` → `member` and `Customer` → `casual`
6. Created `ride_length` column — duration in minutes
7. Created `day_of_week`, `day_name`, `month`, and `hour` columns
8. Removed rides under 1 minute (docking errors)
9. Removed rides over 1,440 minutes / 24 hours (lost or stolen bikes)

Result:783,000+ clean rows ready for analysis

Key Findings
Finding 1 — Casual Riders Take Much Longer Rides
Annual members average approximately 10–12 minutes per ride
Casual riders average approximately 35–45 minutes per ride
Casual riders take 3 to 4 times longer rides than members
This strongly indicates members use bikes for commuting while casuals ride for leisure

Finding 2 — Members Ride on Weekdays, Casuals on Weekends
Member rides peak Tuesday to Thursday and drop sharply on weekends
Casual rider rides are lowest mid-week and peak on Saturday and Sunday
Classic commuter vs. leisure behavioural split confirmed

Finding 3 — Members Show Rush-Hour Peaks, Casuals Do Not
Member rides spike sharply at 8 AM and 5 PM — classic commuting times
Casual rides build gradually and peak around midday (11 AM – 2 PM)
No rush-hour spikes exist in casual rider data — confirms recreational use

Finding 4 — Casual Riders Concentrate at Leisure Locations
Top casual rider start stations are near parks, the lakefront, and tourist attractions
Top member start stations are near offices, residential areas, and transit hubs
Geographic difference confirms where to target marketing materials

Top 3 Recommendations

Recommendation 1 — Weekend Digital Campaign
Based on: Finding 2 — Casual riders peak on weekends

Run targeted digital ads on Friday evenings and Saturday mornings
when casual riders are most likely planning a ride.

Key message:"You ride every weekend — an annual membership pays 
for itself in just a few weekends. Stop buying day passes."

Channels: Instagram, Facebook Ads — targeted by Chicago location

Recommendation 2 — Station-Based Physical Marketing
Based on: Finding 4 — Casuals use parks and tourist locations

Place membership posters, QR code stands, and flyers at the 
Top 10 casual rider start stations.

These are the exact locations where casual riders make their riding 
decisions — meeting them there is far more effective than generic ads.

Action: QR codes linking directly to a discounted membership page

Recommendation 3 — Leisure-to-Commute Conversion Campaign
Based on: Finding 3 — Members use bikes for commuting

Many casual riders do not realise Cyclistic works for daily commuting. 
Create a campaign showing the cost saving of membership vs. public transport.

Key message: "Members commute daily AND stay fit — from just $X per year"

Target: Casual riders who start near business districts

Conclusion

The analysis reveals four clear and consistent behavioral differences 
between Cyclistic's annual members and casual riders.

Members use the service as a commuting and utility tool
short, frequent, weekday trips during rush hours, starting near offices.

Casual riders use the service for leisure and recreation 
long, relaxed rides on weekends and midday, starting at parks and 
tourist attractions.

This behavioral gap is not a barrier to conversion — it is an 
opportunity. Casual riders already know and use Cyclistic. 
The three recommendations above are designed to show them the 
additional value of annual membership in terms they already relate to.

The data is clear. The opportunity is real. The path to conversion 
begins with meeting casual riders where they already are.

About the Author

Nene Perpetual Okogo
BI & Data Analytics Officer | Data Analyst  

okogonene11@gmail.com  
[LinkedIn](https://www.linkedin.com/in/nene-perpetual-okogo)  
[GitHub](https://github.com/NeneOkogo)  

Data License
The datasets are made available by Motivate International Inc. 
under a public data license. This project is for educational and 
portfolio purposes only.

Completed as part of the Google Data Analytics Professional Certificate — 2026
