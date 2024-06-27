# E-Commerece Web Traffic and User Behavior Analysis

# Introduction

This project focuses on analyzing web traffic and user behavior on an e-commerce website. The goal is to identify key metrics and trends that inform decision-making processes, improve user engagement, and increase conversion rates. The analysis will encompass various aspects of user interactions, including page views, sessions, bounce rates, exit rates and average session durations.

## Tools used
1) Microsoft Excel 2016.
2) Power Quer for data extraction, cleaning and prepration.
3) Pivot Tables for analysis and insights.

## Business Questions and Tasks

1) **Comparative Analysis**
    * **Year-over-Year (YoY) Comparison:** Compare metrics from the same periods in different years to assess growth or decline.
    * **Month-over-Month (MoM) Comparison:** Analyze monthly changes to understand short-term trends.

2) **Trend and Time Series Analysis**
    * **Seasonal Trends:** Identify patterns over different times of the year (Year, Month) to understand high and low traffic periods.
    * **Time Series Forecasting:** Use models like ARIMA, SARIMA, or Prophet to predict future web traffic metrics.

## Data cleaning and preparatrion

After cleaning, preparing and understanding the data found the following notes

1) The dataset includes 1826 records.
2) No missing values.
3) Outliers detected inseveral columns (**Page_Views: 1 outlier detected, Bounces: 18 outlers detected and Exits: 34 outliers detected**).
4) Outliers fixed with the **imputation** with the **median** value for each column.
5) New features were generated **Year, Month, Month ID, Weekday and Weekday ID**.
6) KPIs and Metrics calculated (**Total Visits, Total Page Views, Total Sessions, Total Visitors, Total Bounces, Total Exits, Unique Visitors, Repeated Visitors, Repeat visitor rate, Bounce Rate, Exit Rate, Pages per Session, Pages per Visit, Daily Session Duration and Average Session Duration**).
7) The dataset contains 28 features.

## Data Features								

| Column | Count | Type |
| ------ | ----- | ---- |
| Date | 1826 | DATE |
| Visits | 1826 | NUMBER |
| Visitors | 1826 | TEXT |
| Page_Views | 1826 | NUMBER |
| Sessions | 1826 | NUMBER |
| Session_Duration | 1826 | NUMBER |
| Bounces | 1826 | NUMBER |
| Exits | 1826 | NUMBER |
| Year | 1826 | NUMBER |
| Month | 1826 | TEXT |
| Weekday | 1826 | TEXT |
| Month ID | 1826 | NUMBER |
| Weekday ID | 1826 | NUMBER |
| Total Visits | 1826 | NUMBER |
| Total Page Views | 1826 | NUMBER |
| Total Sessions | 1826 | NUMBER |
| Total Visitors | 1826 | NUMBER |
| Total Bounces | 1826 | NUMBER |
| Total Exits | 1826 | NUMBER |
| Unique Visitors | 1826 | NUMBER |
| Repeated Visitors | 1826 | NUMBER |
| Repeat visitor rate | 1826 | PERCENTAGE |
| Bounce Rate | 1826 | PERCENTAGE |
| Exit Rate | 1826 | PERCENTAGE |
| Pages per Session | 1826 | NUMBER |
| Pages per Visit | 1826 | NUMBER |
| Daily Session Duration | 1826 | NUMBER |
| Average Session Duration | 1826 | NUMBER |

## Conclusions
![kpis](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/1.kpis.jpg)
1) key performance indicators (KPIs):
    * total_visits: 9,843,448 visits.
    * total_page_views: 20,484,697 views.
    * total_sessions: 9,860,207 sessions.
    * total_visitors: 1,826 visitors.
    * unique_visitors: 1,621 visitors.
    * repeated_visitors: 205 visitors.
    * total_bounces: 3,359,650 bounces.
    * totsl_exits: 3,886,878 exits.
    * avg_session_duration: 751.96 seconds.
    * bounce_rate: 34.13%.
    * exit_rate: 18.97%.
    * repeat_visitor_rate: 11.23%.
    * pages_per_session: 2.08 pages.
    * pages_per_visit: 2.08 pages.

2) Based on the data provided for the Year-over-Year analysis, The following insights were found:
    ![total_visits_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/2.total_visits_by_year.jpg)
    * **2019 to 2020:** There was a significant **increase** of approximately **9.52%** in total visits, This could be attributed to a variety of factors, including an increase in online activity due to the COVID-19 pandemic.
    * **2020 to 2021:** A **decrease** of about **-4.92%**, This might indicate a stabilization or a slight decline in web traffic as the initial surge in online activity due to the pandemic started to normalize.
    * **2021 to 2022:** A further slight **decrease** of about **-0.81%**, indicating a continued but small decline in visits.
    * **2022 to 2023:** A marginal **increase** of about **0.31%**, suggesting a possible stabilization of visits.
    * The notable **increase** in **2020** could be heavily influenced by the global COVID-19 pandemic, which drove more users online. This is a common trend seen across various ecommerce platforms during that period.
    * The slight **decline** in subsequent years (**2021 and 2022**) might suggest a normalization of online shopping behavior as the pandemic's impact lessened, and offline shopping resumed.
    ![total_page_views_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/3.total_page_views_by_year.jpg)
    * **2019 to 2020:** There was an **increase** of approximately **7.3%** in total page views. This aligns with the trend observed in total visits, likely influenced by the COVID-19 pandemic increasing online activity.
    * **2020 to 2021:** A slight **decrease** of about **-1.36%**, indicating a possible stabilization or slight reduction in user engagement.
    * **2021 to 2022:** A further **decrease** of approximately **-1.37%**.
    * **2022 to 2023:** Another **decrease** of about **-1.26%**, showing a consistent, though gradual, decline over the last three years.
    * The trends in **page views** closely mirror those in **total visits**, with a **peak** in **2020** followed by slight **declines** in subsequent years.
    * While the number of visits to the site has stabilized or slightly decreased, the number of pages viewed per visit has remained relatively consistent.
    ![total_sessions_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/4.total_sessions_by_year.jpg)
    * **2019 to 2020:** There was a significant **increase** of approximately **9.89%** in total sessions. This aligns with the increase observed in visits and page views, likely due to the COVID-19 pandemic driving more online activity.
    * **2020 to 2021:** A **decrease** of about **-4.41%**, indicating a normalization or slight decline post the initial pandemic surge.
    * **2021 to 2022:** A slight **decrease** of approximately **-0.70%**, suggesting a continued stabilization.
    * **2022 to 2023:** Sessions remained almost flat with a **negligible increase** of about **0.01%**, indicating a stable trend.
    * The trends in **sessions** closely mirror those in **total visits** and **page views**, with a peak in **2020** followed by slight declines in subsequent years.
    * While the overall user engagement (in terms of sessions) has seen a minor decline **post-2020**, it has stabilized in the recent years (**2022 and 2023**).
    ![total_bounces_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/5.total_bounces_by_year.jpg)
    * **2019 to 2020:** There was a significant **increase** in total bounces, from **634,573** to **723,015** which a **13.94% increase**, indicating a rise in single-page sessions where users exited without further interaction, This increase could be attributed to various factors such as changes in site usability, content relevance, or user behavior shifts.
    * **2020 to 2021:** A **decrease** in total bounces was observed, dropping from **723,015** to **667,104** which a **decrease** by **-7.71%**. This suggests that efforts might have been made to improve user engagement or address issues that led to higher bounce rates in the previous year.
    * **2021 to 2022:** There was a slight **decrease** in total bounces from **667,104** to **663,082** representing a **-0.60% decrease**, indicating that the trend of reducing bounce rates continued.
    * **2022 to 2023:** A small **increase** in total bounces occurred, from **663,082** to **671,876** (**1.33% increase**). This suggests a potential stabilization or minor regression in addressing bounce rate issues.
    ![bounce_rate_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/6.bounce_rate_by_year.jpg)
    * **2019 to 2020:** There was an **increase** in bounce rate from **33.56%** to **34.91%**, indicating that more visitors left the site after viewing a single page in **2020** compared to **2019**. This increase might be due to various factors such as changes in website design, content quality, or external factors affecting user behavior.
    * **2020 to 2021:** The bounce rate decreased from **34.91%** to **33.88%**, suggesting improvements in user engagement or site optimization efforts. This reduction is positive as it indicates that fewer visitors are leaving the site without further interaction.
    * **2021 to 2022:** The bounce rate increased slightly from **33.88%** to **33.95%**, which is a minor change. This could indicate stabilization or a slight regression in retaining visitors on the site.
    * **2022 to 2023:** The bounce rate increased again from **33.95%** to **34.29%**, This increase suggests a potential challenge in maintaining user engagement or addressing issues that could lead to higher bounce rates.
    ![total_exits_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/7.total_exits_by_year.jpg)
    * **2019 to 2020:** There was an **increase** in total exits from **755,513** to **804,919** which represents a **6.54%**, indicating more users left the site in **2020** compared to **2019**, This increase could be due to various reasons such as changes in user behavior, site content, or external factors like the pandemic which altered online browsing patterns.
    * **2020 to 2021:** The total exits decreased with **-3.48%** to **776,901**, suggesting that efforts to retain users on the site were somewhat successful, though the total exits remained higher than in 2019.
    * **2021 to 2022:** A slight **decrease** of **-0.31%** totaling **774,464** exits , indicating stabilization in user exit behavior.
    * **2022 to 2023:** The total exits remained nearly flat with a very small increase to **775,081** which represents a **0.08%**, suggesting a stable exit pattern.
    ![exit_rate_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/8.exit_rate_by_year.jpg)
    * **2019 to 2020:** There was a slight **decrease** in exit rate from **19.20%** to **19.06%**. This suggests a small improvement in user retention, as a slightly lower percentage of visitors exited the site after viewing any page.
    * **2020 to 2021:** The exit rate further **decreased** to **18.66%**. This indicates a more substantial improvement in retaining visitors, potentially due to improvements in user experience, content quality, or navigation.
    * **2021 to 2022**: The exit rate **increased** slightly to **18.85%**. While still lower than **2019**, this slight increase may suggest minor issues in user experience or content that led to more exits.
    * **2022 to 2023:** The exit rate **increased** again to **19.11%**, approaching the 2019 level. This suggests a regression in user retention, indicating potential areas for improvement to reduce exits.
    ![avg_session_duration_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/9.avg_session_duration_by_year.jpg)
    * **2019 to 2020:** There was a slight **decrease** in average session duration from **756.68** seconds to **748.42** seconds. This indicates that users spent slightly less time per session in **2020** compared to **2019**.
    * **2020 to 2021:** The average session duration **increased** to **753.30** seconds. This suggests that user engagement improved, with users spending more time per session in **2021**.
    * **2021 to 2022:** There was another slight **decrease** to **747.06** seconds. This indicates a drop in user engagement in terms of session duration.
    * **2022 to 2023:** The average session duration **increased** again to **754.36** seconds. This suggests an improvement in user engagement, with users spending more time on the site per session.
    ![pages_per_session_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/10.pages_per_session_by_year.jpg)
    * **2019 to 2020:** There was a slight **decrease** in pages per session from **2.09** to **2.04**. This indicates that users viewed slightly fewer pages per session in **2020** compared to **2019**.
    * **2020 to 2021:** The pages per session **increased** to **2.11**. This suggests an improvement in user engagement, with users viewing more pages per session in **2021**.
    * **2021 to 2022:** There was a minor **decrease** back to **2.09**, indicating a slight drop in the number of pages viewed per session.
    * **2022 to 2023:** The pages per session **decreased** slightly again to **2.06**. This suggests a continuing trend of minor fluctuations in user engagement.
    ![pages_per_visit_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/11.pages_per_visit_by_year.jpg)
    * **2019 to 2020:** There was a slight **decrease** in pages per visit from **2.08** to **2.04**. This indicates that users viewed fewer pages per visit in **2020** compared to **2019**, which might suggest changes in user behavior, content relevance, or site navigation.
    * **2020 to 2021:** The pages per visit **increased** to **2.11**, showing an improvement in user engagement with users viewing more pages per visit in **2021**.
    * **2021 to 2022:** There was a slight **decrease** to **2.10** pages per visit, indicating a minor drop in user engagement.
    * **2022 to 2023:** The pages per visit **decreased** again to **2.07**, continuing the trend of minor fluctuations in user engagement.
    ![repeated_visitors_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/12.repeated_visitors_by_year.jpg)
    * **2019 to 2020:** There was a slight **decrease** in repeated visitors from **11** to **10**, indicating a small drop in the number of users returning to the site.
    * **2020 to 2021:** The number of repeated visitors **decreased** significantly from **10** to **6**. This substantial drop suggests that fewer users found reasons to return to the site in **2021**.
    * **2021 to 2022:** The number of repeated visitors **increased** to **10**, indicating a recovery in user retention and suggesting improvements in user engagement or satisfaction.
    * **2022 to 2023:** The number of repeated visitors **decreased** again to **5**, which is the lowest in the observed period. This suggests significant challenges in retaining users and encouraging return visits.
    ![repeat_visitor_rate_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/13.repeat_visitor_rate_by_year.jpg)
    * **2019 to 2020:** The repeat visitor rate **decreased** from **3.01%** to **2.73%**, indicating a slight drop in the proportion of visitors returning to the site.
    * **2020 to 2021:** There was a significant **decrease** to **1.64%**, suggesting a notable decline in user retention and satisfaction.
    * **2021 to 2022:** The repeat visitor rate **increased** to **2.74%**, showing a recovery in the proportion of returning visitors, possibly due to improved engagement strategies or better user experience.
    * **2022 to 2023:** The rate **decreased** again to **1.37%**, indicating substantial challenges in retaining visitors and encouraging them to return.
    ![total_visitors_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/14.total_visitors_by_year.jpg)
    * The total number of visitors remains remarkably stable across the years, with a negligible change (**only one additional visitor in 2020**). This indicates that the website attracts a consistent number of visitors each year.
    ![unique_visitors_by_year](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/15.unique_visitors_by_year.jpg)
    * There is a gradual **increase** in the number of unique visitors from **2019** to **2023**. While the increase is modest, it suggests a positive trend in attracting new unique visitors to the website each year.
    * Traffic Metrics (Visits, Page Views, and Sessions):
        * **2020:** All three metrics show a peak in 2020, likely influenced by increased online activity due to the pandemic.
        * **2021-2023:** There's a stabilization or slight decline in all metrics, suggesting normalization post-pandemic.
    * Engagement Metrics (Average Session Duration, Pages per Session and Pages per Visit):
        * **2020:** Both pages per session and pages per visit decreased, suggesting users viewed fewer pages during their visits despite the increase in total visits and sessions.
        * **2021:** An increase in pages per session and pages per visit coincides with an increase in average session duration, indicating improved user engagement.
        * **2022-2023:** Minor fluctuations, with a slight decrease in pages per session and pages per visit, suggesting a slight decline in user engagement.
    * Exit and Bounce Metrics (Total Bounces, Bounce Rate, Total Exits and Exit Rate):
        * **2020:** The bounce rate and total bounces increased significantly, suggesting that while more people visited the site, many left quickly without interacting further.
        * **2021:** Improvement seen as both total bounces and bounce rate decreased.
        * **2022-2023:** Bounce rate and total bounces show a slight increase, indicating potential issues with user engagement or satisfaction.
        * Exit rates are relatively stable, suggesting consistent behavior in terms of how users leave the site.
    * Repeat Visitor Metrics (Repeated Visitors and Repeat Visitor Rate):
        * **2019 to 2020:** A slight decrease in repeat visitor metrics, but still relatively stable.
        * **2021:** Significant drop in both repeated visitors and repeat visitor rate, suggesting a major decline in user retention.
        * **2022:** Temporary recovery in repeat visitors and repeat visitor rate, indicating successful re-engagement efforts.
        * **2023:** Significant decline again, highlighting ongoing challenges in retaining users.
    * **Traffic and Engagement:** The peak in traffic metrics (visits, page views, sessions) in 2020 did not correlate with improved engagement metrics (pages per session, pages per visit, average session duration), suggesting that increased traffic did not necessarily lead to deeper engagement.
    * **Bounce and Exit Rates:** The increase in bounce rate and total bounces in 2020 indicates that despite higher traffic, users were not finding the content engaging or relevant. This trend is partially improved in 2021, but bounces and exits remain a concern.
    * **Retention Challenges:** The drop in repeat visitors and repeat visitor rate in 2021 and 2023 suggests that user retention is a significant issue. Even if users spend more time on the site (as seen with average session duration), they are not necessarily returning, indicating a need for better re-engagement strategies.
    * **Engagement Correlation:** The slight improvements in 2021 in pages per session, pages per visit, and average session duration indicate that targeted efforts to improve content or user experience can positively impact user engagement.

4) Based on the data provided for the Month-over-Month analysis here are the observations found:
   ![2019_total_visits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/16.2019_total_visits_by_month.jpg)
    * In **2019**:
        * **February**: Significant drop (**-12.47%**), aligning with the low seasonality index.
        * **March**: Strong recovery (**35.11%**), reflecting a seasonal rebound.
        * **August**: Highest MoM growth (**28.67%**), matching its high seasonality index.
    ![2020_total_visits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/17.2020_total_visits_by_month.jpg)
    * In **2020**:
        * **February**: Decline (**-3.19%**), but less severe than in **2019**.
        * **March**: Positive growth (**17.60%**), following the seasonal trend.
        * **April**: Sharp decline (**-16.13%**), indicating potential post-March drop-off.
        * **November**: Significant decline (**-13.20%**), could be due to pre-holiday season slowdown.
    ![2021_total_visits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/18.2021_total_visits_by_month.jpg)
    * In **2021**:
        * **February** and **March**: Continuous decline, significant in **March** (**-17.34%**).
        * **April**: Recovery (**19.19%**), consistent with post-March rebound.
        * **June**: Strong positive growth (**12.46%**), higher than average.
    ![2022_total_visits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/19.2022_total_visits_by_month.jpg)
    * In **2022**:
        * **January** to **February**: Major decline (**-23.98%**), sharper than previous years.
        * **August**: Strong positive growth (**19.37%**), reflecting seasonal peak.
        * **October**: Significant growth (**16.23%**), high seasonality impact.
    ![2023_total_visits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/20.2023_total_visits_by_month.jpg)
    * In **2023**:
        * **February**: Sharp decline (**-27.68%**), largest drop observed, aligning with low seasonality.
        * **March**: Strongest recovery (**38.37%**), indicating a robust seasonal effect.
        * **May** to **June**: Positive growth, but declining slightly by December.
    ![visits_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/21.visits_seasonality_index_by_month.jpg)
    * There is a noticeable volatility in MoM growth across all years, with significant fluctuations in certain months. For example, **February** generally shows negative growth, while **March** often sees a rebound.
    * **August** frequently exhibits positive MoM growth, reflecting a seasonal increase in visits during this month.
    * **August** (S.I. **1.09**) and **January** (S.I. **1.05**) are months with higher-than-average visits, while **February** (S.I. **0.88**) consistently shows lower-than-average visits.
    * **February** shows a consistent decline in visits across multiple years. This aligns with its low seasonality index of **0.88**.
    * **March** consistently rebounds from **February’s** decline, as indicated by positive MoM growth in multiple years and a seasonality index of **1.03**.
    ![2019_page_views_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/22.2019_page_views_by_month.jpg)
    * In **2019**:
        * High Page Views: **February** (**420,238**) and **November** (**339,533**) had the highest page views.
        * Low Page Views: **April** (**261,649**) and **September** (**293,256**) had the lowest page views.
        * Seasonality Impact: **February** and **November** are in line with their high S.I., while **April** and **September** match their low S.I.
    ![2020_page_views_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/23.2020_page_views_by_month.jpg)
    * In **2020**:
        * High Page Views: **August** (**397,048**) and **November** (**384,747**) had the highest page views.
        * Low Page Views: **October** (**307,196**) and **April** (**371,143**) had the lowest page views.
        * Seasonality Impact: **August** and **November** align with high S.I., but **October** is unexpectedly low despite an average S.I.
    ![2021_page_views_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/24.2021_page_views_by_month.jpg)
    * In **2021**:
        * High Page Views: **February** (**398,881**) and **July** (**403,251**) had the highest page views.
        * Low Page Views: **August** (**279,274**) and **December** (**322,225**) had the lowest page views.
        * Seasonality Impact: **February** and **July** align with their S.I., but ***August*** is lower than expected.
    ![2022_page_views_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/25.2022_page_views_by_month.jpg)
    * In **2022**:
        * High Page Views: **May** (**413,352**) and **January** (**370,351**) had the highest page views.
        * Low Page Views: **April** (**278,399**) and **June** (**293,757**) had the lowest page views.
        * Seasonality Impact: **May** aligns with a high S.I., while **April** is low as expected.
    ![2023_page_views_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/26.2023_page_views_by_month.jpg)
    * In **2023**:
        * High Page Views: **February** (**396,295**) and **November** (**359,664**) had the highest page views.
        * Low Page Views: **April** (**245,938**) and **May** (**303,000**) had the lowest page views.
        * Seasonality Impact: **February** and **November** are consistent with their high S.I., while **April** matches its low S.I.
    ![page_views_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/27.page_views_seasonality_index_by_month.jpg)
    * Page views fluctuate month by month, with some months showing consistent increases or decreases across multiple years.
    * **February** and **March** generally show higher page views, while **April** tends to have lower page views.
    * **February** (S.I. **1.14**) and **November** (S.I. **1.04**) are months with higher-than-average page views, indicating seasonal peaks.
    * **April** (S.I. **0.89**) and **September** (S.I. **0.95**) consistently have lower page views, indicating potential seasonal dips.
    ![2019_sessions_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/28.2019_sessions_by_month.jpg)
    * In **2019**:
        * High Sessions: **March** (**173,168**), **August** (**194,008**), and **December** (**171,995**) had the highest sessions.
        * Low Sessions: **February** (**128,556**) and **July** (**147,710**) had the lowest sessions.
        * Seasonality Impact: **August** aligns with its high S.I., and **February** aligns with its low S.I.
    ![2020_sessions_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/29.2020_sessions_by_month.jpg)
    * In **2020**:
        * High Sessions: **March** (**200,757**), **October** (**190,650**), and **January** (**172,140**) had the highest sessions.
        * Low Sessions: **December** (**149,342**) and **May** (**158,296**) had the lowest sessions.
        * Seasonality Impact: **March** and **October** align with their high S.I., while **December** is unexpectedly low despite an average S.I.
    ![2021_sessions_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/30.2021_sessions_by_month.jpg)
    * In **2021**:
        * High Sessions: **January** (**186,718**) and **June** (**190,675**) had the highest sessions.
        * Low Sessions: **February** (**159,729**) and **September** (**145,994**) had the lowest sessions.
        * Seasonality Impact: **January** aligns with its high S.I., and **February** aligns with its low S.I.
    ![2022_sessions_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/31.2022_sessions_by_month.jpg)
    * In **2022**:
        * High Sessions: **January** (**194,455**) and **October** (**180,216**) had the highest sessions.
        * Low Sessions: **February** (**141,345**) and **July** (**144,992**) had the lowest sessions.
        * Seasonality Impact: **January** and **October** align with their high S.I., while **February** aligns with its low S.I.
    ![2023_sessions_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/32.2023_sessions_by_month.jpg)
    * In **2023**:
        * High Sessions: **November** (**180,984**) and **June** (**176,242**) had the highest sessions.
        * Low Sessions: **February** (**119,489**) and **September** (**159,482**) had the lowest sessions.
        * Seasonality Impact: **November** and **June** align with their high S.I., while **February** aligns with its low S.I.
    ![sessions_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/33.sessions_seasonality_index_by_month.jpg)
    * Sessions fluctuate month by month, with some months showing consistent increases or decreases across multiple years.
    * **August**, **October**, and **January** generally show higher sessions, while **February** consistently has lower sessions.
    * **August** (S.I. **1.09**) and **October** (S.I. **1.07**) have higher-than-average sessions, indicating seasonal peaks.
    * **February** (S.I. **0.88**) consistently has lower sessions, indicating a potential seasonal dip.
    ![2019_bounces_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/34.2019_bounces_by_month.jpg)
    * In **2019**:
        * High Bounces: **March** (**60,136**), **August** (**64,302**), and **December** (**59,468**) had the highest bounces.
        * Low Bounces: **February** (**40,230**) and **April** (**49,266**) had the lowest bounces.
        * Seasonality Impact: **August** and **October** align with their high S.I., and **February** aligns with its low S.I.
    ![2020_bounces_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/35.2020_bounces_by_month.jpg)
    * In **2020**:
        * High Bounces: **March** (**67,428**), **October** (**67,896**), and **January** (**62,024**) had the highest bounces.
        * Low Bounces: **December** (**49,903**) and **May** (**56,107**) had the lowest bounces.
        * Seasonality Impact: **March** and **October** align with their high S.I., while **December** is unexpectedly low despite an average S.I.
    ![2021_bounces_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/36.2021_bounces_by_month.jpg)
    * In **2021**:
        * High Bounces: **January** (**60,346**) and **June** (**63,758**) had the highest bounces.
        * Low Bounces: **March** (**42,767**) and **September** (**47,947**) had the lowest bounces.
        * Seasonality Impact: **January** aligns with its high S.I., and **February** aligns with its low S.I.
    ![2022_bounces_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/37.2022_bounces_by_month.jpg)
    * In **2022**:
        * High Bounces: **January** (**67,890**) and **November** (**57,506**) had the highest bounces.
        * Low Bounces: February (**50,636**) and **September** (**49,520**) had the lowest bounces.
        * Seasonality Impact: **January** and **November** align with their high S.I., while **February** aligns with its low S.I.
    ![2023_bounces_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/38.2023_bounces_by_month.jpg)
    * In **2023**:
        * High Bounces: **June** (**65,015**) and **October** (**61,942**) had the highest bounces.
        * Low Bounces: **February** (**42,779**) and **September** (**52,428**) had the lowest bounces.
        * Seasonality Impact: **June** and **October** align with their high S.I., while **February** aligns with its low S.I.
    ![bounces_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/39.bounces_seasonality_index_by_month.jpg)
    * Bounces fluctuate month by month, with some months showing consistent increases or decreases across multiple years.
    * **February** consistently shows lower bounces, while **August** and **October** generally have higher bounces.
    * **August** (S.I. **1.08**) and **October** (S.I. **1.08**) have higher-than-average bounces, indicating seasonal peaks.
    * **February** (S.I. **0.87**) consistently has lower bounces, indicating a potential seasonal dip.
    ![2019_bounce_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/40.2019_bounce_rate_by_month.jpg)
    * In **2019**:
        * High Bounce Rates: **March** (**34.40%**), **July** (**34.53%**), and **October** (**34.91%**) had the highest bounce rates.
        * Low Bounce Rates: **January** (**30.87%**) and **February** (**31.09%**) had the lowest bounce rates.
        * Seasonality Impact: The high bounce rates in **March**, **July**, and **October** are consistent with their seasonality indices, which are close to or above 1.
    ![2020_bounce_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/41.2020_bounce_rate_by_month.jpg)
    * In **2020**:
        * High Bounce Rates: **January** (**35.32%**), **July** (**37.40%**), and **October** (**36.91%**) had the highest bounce rates.
        * Low Bounce Rates: **February** (**33.49%**) and **December** (**32.98%**) had the lowest bounce rates.
        * Seasonality Impact: **July** and **October** align with their high S.I., while **December** aligns with its low S.I.
    ![2021_bounce_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/42.2021_bounce_rate_by_month.jpg)
    * In **2021**:
        * High Bounce Rates: **April** (**36.74%**) and **November** (**35.46%**) had the highest bounce rates.
        * Low Bounce Rates: **March** (**32.23%**) and **September** (**31.05%**) had the lowest bounce rates.
        * Seasonality Impact: **April** and **November** align with their high S.I., while **March** and **September** align with their low S.I.
    ![2022_bounce_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/43.2022_bounce_rate_by_month.jpg)
    * In **2022**:
        * High Bounce Rates: **May** (**37.05%**) and **November** (**36.13%**) had the highest bounce rates.
        * Low Bounce Rates: **March** (**32.55%**) and **October** (**31.81%**) had the lowest bounce rates.
        * Seasonality Impact: **May** and **November** align with their high S.I., while **March** and **October** are unexpectedly lower despite high S.I.
    ![2023_bounce_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/44.2023_bounce_rate_by_month.jpg)
    * In **2023**:
        * High Bounce Rates: **June** (**36.73%**) and **October** (**36.79%**) had the highest bounce rates.
        * Low Bounce Rates: **July** (**31.83%**) and **November** (**32.29%**) had the lowest bounce rates.
        * Seasonality Impact: **June** and **October** align with their high S.I., while **July** and **November** are unexpectedly lower despite high S.I.
    ![bounce_ratte_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/45.bounce_ratte_seasonality_index_by_month.jpg)
    * Bounce rates vary month by month, with some months showing consistent increases or decreases across multiple years.
    * There are noticeable fluctuations, with **July** and **October** generally having higher bounce rates and **March** and **September** typically having lower bounce rates.
    * **May** (S.I. **1.03**) and **October** (S.I. **1.03**) tend to have higher bounce rates, indicating possible seasonal challenges.
    * **December** (S.I. **0.97**) typically has a lower bounce rate, suggesting higher user engagement during this month.
    ![2019_exits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/46.2019_exits_by_month.jpg)
    * In **2019**:
        * High Exits: **August** (**77,748**), **October** (**69,162**), and **December** (**67,773**) had the highest exits.
        * Low Exits: **June** (**48,995**) and **February** (**53,511**) had the lowest exits.
        * Seasonality Impact: **August** and **October** align with their high S.I., and **February** aligns with its low S.I.
    ![2020_exits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/47.2020_exits_by_month.jpg)
    * In **2020**:
        * High Exits: **October** (**82,739**), **March** (**74,629**), and **February** (**75,372**) had the highest exits.
        * Low Exits: **November** (**57,532**) and **December** (**60,731**) had the lowest exits.
        * Seasonality Impact: **October** aligns with its high S.I., while **February** is unexpectedly high despite a low S.I.
    ![2021_exits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/48.2021_exits_by_month.jpg)
    * In **2021**:
        * High Exits: **August** (**73,410**) and **July** (**70,499**) had the highest exits.
        * Low Exits: **March** (**52,980**) and **February** (**60,548**) had the lowest exits.
        * Seasonality Impact: **August** aligns with its high S.I., and **February** aligns with its low S.I.
    ![2022_exits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/49.2022_exits_by_month.jpg)
    * In **2022**:
        * High Exits: **January** (**71,899**) and **October** (**65,389**) had the highest exits.
        * Low Exits: **February** (**52,209**) and **July** (**54,095**) had the lowest exits.
        * Seasonality Impact: **January** and **October** align with their high S.I., while **February** aligns with its low S.I.
    ![2023_exits_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/50.2023_exits_by_month.jpg)
    * In **2023**:
        * High Exits: **July** (**76,831**) and **August** (**75,079**) had the highest exits.
        * Low Exits: **February** (**44,680**) and **January** (**55,599**) had the lowest exits.
        * Seasonality Impact: **July** and **August** align with their high S.I., while **February** aligns with its low S.I.
     ![exits_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/51.exits_seasonality_index_by_month.jpg)
    * Exits vary month by month, with some months showing consistent increases or decreases across multiple years.
    * **August** generally shows the highest exits, while **February** consistently has lower exits.
    * **August** (S.I. **1.12**) and **October** (S.I. **1.05**) tend to have higher exits, indicating possible seasonal challenges.
    * **February** (S.I. **0.88**) typically has lower exits, suggesting a period of lower user exits.
    ![2019_exit_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/52.2019_exit_rate_by_month.jpg)
    * In **2019**:
        * High Exit Rates: **May** (**21.47%**), **February** (**20.45%**), and **November** (**20.72%**) had the highest exit rates.
        * Low Exit Rates: **June** (**16.26%**) and **December** (**17.88%**) had the lowest exit rates.
        * Seasonality Impact: **May** and **November** align with their high S.I., and **January** and **December** align with their low S.I.
    ![2020_exit_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/53.2020_exit_rate_by_month.jpg)
    * In **2020**:
        * High Exit Rates: **October** (**21.50%**), **June** (**21.01%**), and **February** (**20.31%**) had the highest exit rates.
        * Low Exit Rates: **May** (**16.39%**) and **July** (**16.41%**) had the lowest exit rates.
        * Seasonality Impact: **October** aligns with its high S.I., while **May** and July are unexpectedly low despite the high S.I.
    ![2021_exit_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/54.2021_exit_rate_by_month.jpg)
    * In **2021**:
        * High Exit Rates: **December** (**20.96%**) and **September** (**19.89%**) had the highest exit rates.
        * Low Exit Rates: **February** (**16.95%**) and **June** (**17.82%**) had the lowest exit rates.
        * Seasonality Impact: **September** and **December** align with their high S.I., while **February** is unexpectedly low despite a higher S.I.
    ![2022_exit_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/55.2022_exit_rate_by_month.jpg)
    * In **2022**:
        * High Exit Rates: **June** (**20.82%**) and **September** (**20.15%**) had the highest exit rates.
        * Low Exit Rates: **January** (**17.39%**) and **December** (**17.04%**) had the lowest exit rates.
        * Seasonality Impact: **June** and **September** align with their high S.I., while **January** and **December** align with their low S.I.
    ![2023_exit_rate_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/56.2023_exit_rate_by_month.jpg)
    * In **2023**:
        * High Exit Rates: **September** (**21.43%**) and **July** (**20.56%**) had the highest exit rates.
        * Low Exit Rates: **October** (**17.44%**) and **February** (**18.17%**) had the lowest exit rates.
        * Seasonality Impact: **September** and **July** align with their high S.I., while **October** is unexpectedly low despite a higher S.I.
    ![exit_rate_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/57.exit_rate_seasonality_index_by_month.jpg)
    * Exit rates vary month by month, with some months showing consistent increases or decreases across multiple years.
    * **September** and **October** generally show higher exit rates, while **January** and **December** tend to have lower exit rates.
    * **September** (S.I. **1.06**) and **October** (S.I. **1.01**) tend to have higher exit rates, indicating possible seasonal challenges.
    * **January** (S.I. **0.97**) and **December** (S.I. **0.97**) typically have lower exit rates, suggesting better user engagement during these months.
    ![2019_avg_session_duartion_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/58.2019_avg_session_duartion_by_month.jpg)
    * In **2019**:
        * High Average Session Durations: **February** (**780.74**) and **August** (**772.68**) had the highest session durations.
        * Low Average Session Durations: **June** (**708.25**) and **November** (**743.80**) had the lowest session durations.
        * Seasonality Impact: **February** and **August** align with their high S.I., while **June** aligns with its low S.I.
    ![2020_avg_session_duartion_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/59.2020_avg_session_duartion_by_month.jpg)
    * In **2020**:
        * High Average Session Durations: **February** (**774.34**) and **July** (**769.41**) had the highest session durations.
        * Low Average Session Durations: **April** (**733.96**) and **December** (**728.20**) had the lowest session durations.
        * Seasonality Impact: **February** aligns with its high S.I., while **December** is unexpectedly low despite the average S.I.
    ![2021_avg_session_duartion_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/60.2021_avg_session_duartion_by_month.jpg)
    * In **2021**:
        * High Average Session Durations: ***December*** (**784.98**) and **March** (**765.06**) had the highest session durations.
        * Low Average Session Durations: **October** (**728.10**) and **July** (**735.42**) had the lowest session durations.
        * Seasonality Impact: **March** and **December** align with their high S.I., while **October** and **July** are unexpectedly low despite the average S.I.
    ![2022_avg_session_duartion_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/61.2022_avg_session_duartion_by_month.jpg)
    * In **2022**:
        * High Average Session Durations: **March** (**785.22**) and **August** (**772.87**) had the highest session durations.
        * Low Average Session Durations: **June** (**724.81**) and **September** (**714.20**) had the lowest session durations.
        * Seasonality Impact: **March** and **August** align with their high S.I., while **June** and **September** align with their low S.I.
    ![2023_avg_session_duartion_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/62.2023_avg_session_duartion_by_month.jpg)
    * In **2023**:
        * High Average Session Durations: **February** (**775.36**) and **September** (**774.18**) had the highest session durations.
        * Low Average Session Durations: **August** (**719.51**) and **June** (**729.81**) had the lowest session durations.
        * Seasonality Impact: **February** and **September** align with their high S.I., while **August** and **June** align with their low S.I.
    ![avg_session_duration_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/63.avg_session_duration_seasonality_index_by_month.jpg)
    * Average session duration varies month by month, with some months showing consistent increases or decreases across multiple years.
    * **February** and **March** generally show higher average session durations, while **June** often has lower average session durations.
    * **February** (S.I. **1.01**) and **March** (S.I. **1.02**) tend to have higher session durations, indicating better user engagement during these months.
    * **June** (S.I. **0.97**) typically has lower session durations, suggesting a period of lower user engagement.
    ![2019_pages_per_session_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/64.2019_pages_per_session_by_month.jpg)
    ![2020_pages_per_session_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/65.2020_pages_per_session_by_month.jpg)
    ![2021_pages_per_session_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/66.2021_pages_per_session_by_month.jpg)
    ![2022_pages_per_session_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/67.2022_pages_per_session_by_month.jpg)
    ![2023_pages_per_session_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/68.2023_pages_per_session_by_month.jpg)
    ![pages_per_session_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/69.pages_per_session_seasonality_index_by_month.jpg)
    * The number of pages per session shows variability across different years. For example, the pages per session in **January** varied from **1.81** in **2023** to **2.36** in **2019**.
    * There is no clear increasing or decreasing trend over the years, indicating fluctuating user engagement.
    * Certain months show consistently higher engagement (more pages per session), such as **August** and **July**, which often have values above **2.0**.
    * Other months like **March** and **May** show relatively lower engagement in some years.
    * High-Engagement Months: **August** (S.I. = **1.05**), **July** (S.I. = **1.02**), **December** (S.I. = **1.03**)
    * Low-Engagement Months: **March** (S.I. = **0.96**), **May** (S.I. = **0.97**), **October** (S.I. = **0.97**)
    ![2019_pages_per_visit_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/70.2019_pages_per_visit_by_month.jpg)
    ![2020_pages_per_visit_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/71.2020_pages_per_visit_by_month.jpg)
    ![2021_pages_per_visit_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/72.2021_pages_per_visit_by_month.jpg)
    ![2022_pages_per_visit_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/73.2022_pages_per_visit_by_month.jpg)
    ![2023_pages_per_visit_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/74.2023_pages_per_visit_by_month.jpg)
    ![pages_per_visit_seasonality_index_by_month](https://github.com/ahadel943/ecommerece_web_traffic_and_user_behavior_analysis/blob/main/charts/75.pages_per_visit_seasonality_index_by_month.jpg)
    * The number of pages per visit shows some variability across different years. For instance, the pages per visit in January varied from **1.82** in **2023** to **2.19** in **2022**.
    * Overall, there seems to be no clear upward or downward trend over the years.
    * Certain months consistently show higher engagement (more pages per visit), such as **August** and **December**, often having values above **2.0**.
    * Other months like **March** and **May** tend to have relatively lower engagement in several years.
    * High-Engagement Months: **August** (S.I. = **1.04**), **December** (S.I. = **1.03**), **April** (S.I. = **1.02**), **July** (S.I. = **1.02**)
    * Low-Engagement Months: **March** (S.I. = **0.97**), **May** (S.I. = **0.97**), **October** (S.I. = **0.98**)
    * Most months have a seasonality index close to **1.00**, indicating relatively stable engagement levels.

6) The following insights were interpretered based on our visits forecasting model:
    * By using a **Seasonal Trend Decomposition using Linear Regression (STDLR)** we were able to build a model which is reasonably accurate with a Mean Absolute Percentage Error (**MAPE**) of **5.93%**.
    * The forecasted visits for 2024<br>
    * | Month | Visits | MoM Grwoth |
      | ----- | ------ | ---------- |
      | January | 173,101 | 0.00%   |
      | February | 145,637 | -15.87% |
      | March | 169,454 | 16.35% |
      | April | 158,725 | -6.33% |
      | May | 161,888 | 1.99% |
      | June | 167,808 | 3.66% |
      | July | 164,774 | -1.81% |
      | August | 180,535 | 9.57% |
      | September | 159,416 | -11.70% |
      | October | 173,981 | 9.14% |
      | November | 161,632 | -7.10% |
      | December | 165,478 | 2.38% |
    * An excpected growth by **1.18%** in **2024**.
    * **February** shows lower visit volumes compared to other months, with a forecast of **145,637** visits in **2024**. This suggests a period where we can plan for maintenance or cost-saving measures.
    * **August** consistently shows high visit volumes. For **2024**, the forecasted visits for **August** are **180,535**. This indicates a peak period where we should ensure maximum resource availability.
    * **January** visits have steadily increased from **147,822** in **2019** to a forecasted **173,101** in **2024**, Except for **2023** there was a dip. This indicates a growth trend.
    * **March** **2024** shows a forecast of **169,454** visits, which is slightly higher compared to **March** **2023** (**169,063** visits), it suggests stable growth.
    * **April 2024** are forecasted at **158,725**, compared to **148,165** in **April 2023**, it suggests an opportunity to capitalize on an expected increase in demand.
    * **November** have a slight forecasted increase (**161,632** in **2024** from **161,259** in **2023**), it indicates stability but also the need to maintain efforts to keep the visits up.

    * By using a **Seasonal Trend Decomposition using Linear Regression (STDLR)** we were able to build a model which is reasonably accurate with a Mean Absolute Percentage Error (**MAPE**) of **6.87%**.
    * The forecasted page views for 2024<br>
    * | Month | Page Views | MoM Grwoth |
      | ----- | ------ | ---------- |
      | January | 334,031 | 0.00%   |
      | February | 388,809 | 16.40% |
      | March | 352,080 | -9.45% |
      | April | 303,787 | -13.72% |
      | May | 349,597 | 15.08% |
      | June | 348,993 | -0.17% |
      | July | 347,807 | -0.34% |
      | August | 339,299 | -2.45% |
      | September | 325,967 | -3.93% |
      | October | 334,424 | 2.59% |
      | November | 354,865 | 6.11% |
      | December | 330,499 | -6.87% |
    * An excpected growth by **1.34%** in **2024**.
    * Certain months consistently show higher seasonal adjusted page views, indicating peak periods for site traffic. For example, **February** and **November** tend to have higher page views.
    * Conversely, months like **April** and **September** tend to have lower page views.
    * In **January**, Page views are relatively stable, with a slight increase expected year-over-year. This indicates a steady start to the year.
    * In **February**, Significant **increase** in page views, suggesting this is a **peak** month. This could be due to specific events, promotions, or user behavior.
    * From **March** to **May**, Page views remain **stable** with slight fluctuations, indicating a consistent user engagement during this period.
    * From **June** to **August**, Slight variations with a **peak** in **June** and relatively stable views in **July** and **August**. This period might be influenced by summer activities or holidays.
    * From **September** to **November**, Gradual **increase** with a **peak** in **November**, indicating another high-traffic period.
    * In **December**, A slight dip, possibly due to holiday seasons where users might be less active online.
    
    * By using a Seasonal Trend Decomposition using Linear Regression (STDLR) we were able to build a model which is reasonably accurate with a Mean Absolute Percentage Error (**MAPE**) of **6.27%**.
    * | Month | Page Views | MoM Grwoth |
      | ----- | ------ | ---------- |
      | January | 173,439 | 0.00%   |
      | February | 145,744 | -15.97% |
      | March | 171,362 | 17.58% |
      | April | 160,357 | -6.42% |
      | May | 162,657 | 1.43% |
      | June | 169,224 | 4.04% |
      | July | 165,652 | -2.11% |
      | August | 180,884 | 9.20% |
      | September | 159,859 | -11.62% |
      | October | 178,492 | 11.66% |
      | November | 164,445 | -7.87% |
      | December | 166,860 | 1.47% |
    * An excpected yearly growth by **1.75%** in **2024**.
    * The highest number of sessions is forecasted in **August** with **180,884** sessions, indicating a seasonal peak.
    * Another peak is observed in **October** with **178,492** sessions.
    * The forecast indicates the lowest number of sessions in **February** with **145,744** sessions, reflecting a seasonal dip
    * The linear trend forecast shows a steady increase in sessions over the year, starting from **166,236** sessions in **January** and reaching **166,921** sessions in **December**. This suggests a slight but steady overall growth in user sessions throughout the year.
    * The seasonal adjusted forecast provides a refined view by accounting for seasonal variations. For instance, while the linear trend forecast for **August** is **166,672** sessions, the seasonal adjusted forecast is significantly higher at **180,884** sessions. This adjustment highlights the importance of considering seasonality in forecasting.

## Recommendations
1) The KPIs calculated offer a comprehensive overview of our website's performance and user behavior, which can be leveraged to make strategic improvements. Here’s how we can exploit these findings:
    1) **Traffic Metrics (Total Visits, Total Page Views, Total Sessions)**
        * **Content Optimization:** Analyze which pages are driving the most traffic and why. Create more content around these topics.
        * **SEO/SEM Strategy:** Continue optimizing for search engines and invest in search engine marketing to maintain and grow traffic.
        * **Campaign Analysis:** Evaluate which marketing campaigns drive the most visits and sessions, and allocate more budget to these successful campaigns.
    2) **Visitor Metrics (Total Visitors, Unique Visitors, Repeated Visitors, Repeat Visitor Rate)**
        * **Retention Campaigns:** Implement loyalty programs, personalized email marketing, and retargeting ads to encourage repeat visits.
        * **User Engagement:** Engage users through social media, newsletters, and community building activities to foster loyalty.
        * **Onboarding Experience:** Improve the onboarding experience for new users to ensure they understand the value of our site and are more likely to return.
    3) **Engagement Metrics (Avg Session Duration, Pages per Session, Pages per Visit)**
        * **Improve Navigation:** Enhance website navigation to make it easier for users to find what they are looking for, encouraging them to view more pages.
        * **Content Quality:** Improve content quality and relevance to keep users engaged for longer periods and encourage them to explore more pages.
        * **Interactive Elements:** Add interactive elements like videos, quizzes, or user-generated content to increase engagement.
    4) **Bounce and Exit Metrics (Total Bounces, Total Exits, Bounce Rate, Exit Rate)**
        * **Landing Page Optimization:** Ensure landing pages are optimized for conversions with clear, compelling calls to action (CTAs) and easy navigation.
        * **Content Relevance:** Align content more closely with user intent to reduce bounce rates. Use A/B testing to find the most effective content and design.
        * **User Feedback:** Collect and analyze feedback to identify pain points leading to high exit rates. Use this information to make targeted improvements.

2) Here are some actionable steps we can take based on the identified trends and insights in our YoY na;ysis:
    1) **Addressing Traffic Fluctuations**
        * **Marketing Campaigns:** Capitalize on months with traditionally high traffic (like March and August) with targeted marketing campaigns, promotions, and special offers.
        * **Content Refresh:** Update content regularly to keep it relevant and engaging, especially during months with typically lower traffic (like February).
        * **SEO and SEM:** Optimize for search engines and invest in search engine marketing to maintain and grow traffic beyond pandemic peaks.
    2) **Improving Engagement**
        * **User Experience (UX) Optimization:** Continuously test and improve website navigation, load times, and mobile responsiveness to enhance user experience.
        * **Personalization:** Use data-driven personalization to show relevant content and product recommendations based on user behavior and preferences.
        * **Content Strategy:** Focus on high-quality, engaging content that encourages users to explore more pages. Consider implementing a blog, video content, and user-generated content.
    3) **Reducing Bounce and Exit Rates**
        * **Landing Page Optimization:** Ensure landing pages are optimized for conversions with clear, compelling calls to action (CTAs) and easy navigation.
        * **Content Relevance:** Align content more closely with user intent to reduce bounce rates. Use A/B testing to find the most effective content and design.
        * **Customer Feedback:** Collect and analyze feedback to identify pain points leading to high exit rates. Use this information to make targeted improvements.
    4) **Enhancing Retention**
        * **Retention Campaigns:** Implement loyalty programs, personalized email marketing, and retargeting ads to encourage repeat visits.
        * **Customer Engagement:** Engage users through social media, newsletters, and community building activities to foster loyalty.
        * **User Onboarding:** Improve the onboarding experience for new users to ensure they understand the value of our site and are more likely to return.
    5) **Leveraging Seasonality**
        * **Seasonal Promotions:** Plan major promotions, product launches, and marketing campaigns around high-traffic months to maximize impact.
        * **Seasonal Content:** Create seasonal content that aligns with user interests and search trends during these periods.
        * **Inventory Planning:** Adjust inventory and logistics planning based on expected seasonal demand to ensure optimal stock levels.

3) The insights derived from the Month-Over-Month (MoM) analysis and seasonal indices provide a detailed understanding of user behavior, traffic patterns, and engagement levels throughout the year. Here’s how we can benefit from these insights to enhance our digital strategy:
    1) **Content Strategy:**
        * **High Engagement Months:** Focus on publishing high-quality content during months with traditionally high engagement (e.g., August, December). Plan key content releases, blog posts, and product launches during these periods to maximize visibility and user interaction.
        * **Low Engagement Months:** Identify months with lower engagement (e.g., February, April) and consider running special campaigns, discounts, or interactive content to boost user interest and activity.
    2) **Marketing Campaigns:**
        * **Peak Months:** Schedule major marketing campaigns, advertisements, and promotions during high-traffic months to ensure maximum reach and effectiveness.
        * **Off-Peak Months:** Utilize targeted marketing strategies to maintain steady traffic. Consider retargeting campaigns, email marketing, and personalized offers to re-engage users during these periods.
    3) **Enhance User Experience:**
        * **Bounce Rate and Exit Rate:** Address high bounce and exit rates in specific months (e.g., July, October). Improve page load times, optimize content relevance, and enhance site navigation to reduce drop-offs.
        * **ession Duration and Pages per Session:** Analyze why certain months have higher or lower session durations and pages per session. Improve content quality, add engaging multimedia elements, and create interactive features to keep users on the site longer.
    4) **Seasonal Personalization:**
        * **Tailored Content:** Use the insights to create season-specific content that resonates with user interests and behaviors during different times of the year.
        * **Engagement Initiatives:** Implement engagement initiatives like contests, quizzes, or live events during months with typically lower engagement to maintain user interest and activity.
    5) **Optimize Resources:**
        * **High-Traffic Periods:** Allocate more resources (e.g., bandwidth, customer support) during peak months to handle increased traffic and ensure smooth user experience.
        * **Low-Traffic Periods:** Use quieter months for website maintenance, updates, and testing new features without disrupting a large number of users.
    6) **Staffing:**
        * **Customer Support:** Increase customer support staffing during high-traffic periods to manage higher volumes of inquiries and provide timely assistance.
        * **Content Creation:** Schedule content creation efforts to align with high-engagement periods, ensuring that fresh and engaging content is ready for publication when user activity is at its peak.
    7) **Competitive Advantage:**
        * **Market Trends:** Stay ahead of competitors by anticipating market trends and user behavior patterns. Use the insights to launch timely campaigns and stay relevant in the market.
        * **User Insights:** Gain deeper insights into our user base’s preferences and behaviors. Tailor our offerings to meet their needs better than our competitors.

4) From the insights interpreted from our forecasting models, Here are how we can use these insights to optimize our business strategies and operations:
    1) **Resource Allocation:**
        * **Peak Periods:** Allocate more resources (staffing, server capacity, inventory) during high traffic periods such as August and October to ensure a smooth customer experience and to handle increased demand.
        * **Low Periods:** During low traffic periods like February, consider scheduling maintenance, updates, or cost-saving measures to minimize the impact on users.
    2) **Marketing and Promotions:**
        * **Targeted Campaigns:**  Plan marketing campaigns around the forecasted peak periods. For instance, increase advertising spend and promotional activities in August and October when traffic is expected to be high.
        * **Retention Strategies:** Use the forecast data to develop strategies to retain customers during low traffic months. Offering special discounts or incentives in February can help maintain engagement.
    3) **Inventory Management:**
        * **Stock Management:** Use the forecasted data to optimize inventory levels. Ensure high-demand products are well-stocked during peak periods to prevent stockouts and overstocking during low periods.
        * **Seasonal Products:** Plan the introduction or promotion of seasonal products based on traffic trends. For example, launching new products or special collections during high traffic months can maximize exposure and sales.
    4) **Customer Experience:**
        * **Enhanced Experience:** During high traffic months, enhance customer service to manage the increased volume of queries and issues. Ensure that website performance is optimal to handle the increased load.
        * **Feedback Collection:** Collect and analyze customer feedback during low traffic months to identify areas for improvement without overwhelming our resources.
    5) **Budget Planning:**
        * **Advertising Budget:** Allocate our advertising budget more effectively by increasing spend during high traffic months and optimizing for cost-efficiency during low traffic periods.
        * **Operational Budget:** Plan our operational budget to ensure sufficient funds are available during peak periods for necessary expenditures like additional staffing or expedited shipping.
    6) **Content Strategy:**
        * **Content Timing:** Align our content strategy with traffic patterns. Publish important content, blogs, or announcements during high traffic periods for maximum reach.
        * **Engagement Content:**  During low traffic periods, focus on engaging content that can drive traffic and keep users engaged, such as quizzes, interactive posts, or user-generated content campaigns.

By effectively leveraging these insights, we can enhance our e-commerce business's overall performance, improve customer satisfaction, and drive sustained growth.
