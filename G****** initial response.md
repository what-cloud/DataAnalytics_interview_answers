Q1:
A: To be honest I primarily use G*****b (competitor), the first time I noticed G***** is probably when the production data**** is dropped hence the live recovery. Your transparency really impressed me. Upon a close look, I found the transparency is inherent, which is my deep belief- a transparent organisation will attract more talent and support and trust from client and partners and even competitors. This is relevant to the product itself, but I can see you breath open and honest, which are key value for any sucessful data projects.


Q2: ....and what are some challenges you faced?

A: I created a suit of tracking and price changing reports for a major traveling services, audiences include Managing Director (very experienced and detail oriented), Head of ******, and ****** analysts. Some challenges: 

We can only query week-to-date data from U* headquarter server (table truncated daily for newest Week-to-date result), and need to re-create daily (e.g. use Today's cumulative result minus yesterday's to get 1 day result), and then manage history data locally. Extract and load is achieved in Alteryx and feeds to Power BI report, both tools allow users to re-configure the business rules easily

Extremely complex Excel pivot table over pivot tables (aggregate lower granularities, then join to other data to vlookup, then aggregate, filter and many to one mapping to get year on year comparison, data copy/pasted from multiple Hyperion query results.) I migrated it to an Alteryx+Power BI combination, also setup as Power Pivot data source for the advanced Excel user to configure his chart of multiple sailings 1 on 1 comparison horizontally with special position requirements.

Also revenue analysts use to copy paste  source data from H******* reports, and write lengthy levels of nested Excel formula to determine if they should change price of a sailing, then set parameters to move price up or down, then update price in  mainframe. I evaluated how practical it is to implement this dynamically and feed to mainframe automatically, and we chose a hybrid approach to get initial benefits by automating data feed-in and use Alteryx and Excel Macro to simplify how user manipulate the data and get price adjustment. (mainframe update remained manual as it involves lots of processes)

Report is well received as it allows users to choose to monitor the combination they need, view gaps between forecasts and balance the resources plan, the automation saves ~ 20 hours weekly to manually producing the results, and utilised Power BI reports to deliver results to a much wider audience (used to be Excel or Tableau reports)





Q3: Explain the typical **** process along with some common problems encounter during a*****s.

A: I normally align with Cross Industry standard process for Data Mining (CRISP-DM), which is the most adopted standard practice. 
I start from Business Understanding, build Data Understanding, then move to the actual data preparation, modeling(reporting), validation and feedback cycle. This enables everything built with the understanding of the business operation and mapped business world to data world properly.

Q4: Common problems 

A: Data quality (sometimes less obvious, such as loyalty card abuse, scam accounts),
Business process changed but downstream data applications not aware of the change (say method of forecast changed so like for like comparison became useless without adjusting)
Models hard to extend, a report model is built for a specific purpose, possible doesn't contain the low level keys needed to link to a new attribute. 
If the above is combined with insufficent documentation (another issue), then this makes analytic work harder to maintain.

After analytical results are released, how to regularly monitor how users are using it (this is essential to get better ROI from analytical work); also for the same report, user may request different views or further customise some metrics - these should be somehow evaluated during design.

Data Inconsistency, how to reconcile between various source systems and manage the difference.



Single Customer View- how to obtain a closer-to-truth view of business data.

Q5 Time had questions?.
A: It happens from time to time. Sometime say if a report is regularly refreshed but regular health check is not done, and data load is incomplete. Depends on the nature of the inquery, if it is requesting relevant information, then I would always ask how the requested information will be used, then determine how best to address the need (i.e. combine with other requirements to create a new report/feature, or make a simple revision); if it is to clarify why the value or the trend looks unusal, I would assess whether there are any recent new business processes or change, or report modification, then drill down to find the root cause or do comparisons to further validate and narrow down the area to evaluate; if the question comes from a new user, I would spend some time with user to ensure he understand the design considerations and criteria 
Q6 Most difficult

When I just joined a telco, I am tasked to reconcile billing system against financial records, this is relevant to revenue leaks of paying more than what we actually consumed, and how annual report should be audited. Initially I tried is to replicate all the actual billing logic that produced each call/text's usage and charge associated, which evolved over years. Although a few SME know most of the rules (as I gradually built the equivalent of rule engine with their help, many times we stuck, search for legacy rules and refine it for the period the inactive rules was applicable), a few hundred accounts still not match exactly after a couple of weeks. After a couple of weeks' attemps, and careful discussion, we allocated the billing system interim records which are stored as json objects, I used the files (some reverse engineering) to extract item billing and build the reconciliation (matched to cent) as needed by accounting.

Also there are various issues such as some special format not well documented (1 hour 45 min is captured as 105, 60+45=105). A changed business over a few years that are stored in database with no single person knows all details, not to say accurate documents, I am able to reconciled it because my ability to derive assumptions from data, especially when there is gap between data and processed that are not fully documented; timely assistance from domain experts to validate my assupmtions and provide what them start to remember as data reveals; and how myself and accountants worked together to find discrepancies and setup plan to addres them.

Q7: books, blogs in past year to improve data knowledge?

sites:Kaggle,DataCastle,KDnuggets
blogs:
https://www.analyticsvidhya.com
https://cooldata.wordpress.com/
http://hamelg.blogspot.com/
http://www.chaosreignswithin.com/
books:
A mathematician's apology
Machines of loving grace
An Introduction to General Systems Thinking
Gödel, Escher, Bach: An Eternal Golden Braid


Delivered a data analyst course (~15 hours) and shared video/workbooks and notes on Github, preparing all the contents greatly improved how I summarise the basics concepts and advanced skills of data analysis, and the methodology and framework, and I experience again how time consuming it can be to build up other people's skillset from introduction

Q8:Please check our main project (https://G*****.com/meltano/analytics/) and find something attracts you. Why did you choose that?

I'd like to get involved in Sheetload, this is a very useful function, as much as we dislike spreadsheets or flat files (can't agree more with what your document says "the minute you load a csv file into the data warehouse it already stale"), we need to live with it and live better with it before it extinguishes.
(A few other things such as snowflake-dbt/macros, Zuora, bamboohr, seems interesting too, so I should be happy to work on most if not all of the projects)

The goal of a (final) _xf dbt model should be a BEAM* table, which means it follows the business event analysis & model structure and answers the who, what, where, when, how many, why, and how question combinations that measure the bus

Finance: https://about.G*****.com/handbook/finance/financial-planning-and-analysis/#manager-financial-planning--analysis

https://blog.getdbt.com/how-we-configure-snowflake/

transform/snowflake-dbt/models/zuora/base/zuora_account.sql
https://G*****.com/G*****-data/analytics/commit/b3160b44fd207e4c52d90493677ec46dda9eafc4 WHy use many case statements???

MR job make: https://G*****.com/G*****-data/analytics/commit/cf7f17f4fd923078d9220c099e24227a4daaea89

https://news.ycombinator.com/item?id=17667399 (fiveTran
https://G*****.com/meltano/meltano/blob/master/README.md#data-science-lifecycle

https://G*****.com/G*****-data/analytics/commit/c10a026dfc19a72fe839259062cebe613c761aec

https://G*****.com/G*****-data/analytics/blob/e752072a1ae89d977e522b807d2e41624b5d24bd/transform/snowflake-dbt/models/G*****_dotcom/xf/G*****_dotcom_events_monthly_active_users.sql

Base Model for G*****.com
