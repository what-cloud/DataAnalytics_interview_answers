Unless the answer contains confidential information explicitly, any questions I was asked, I may post answers here. Your questions may be your IP, but my answer is my IP.

Certifications and skills that might be useful:

SnowPro certification (Snowflake data warehouse) - I found quite a few fin-tech or internet companies using them, such as Gitlab, Prospa, Accenture etc.
Mongo DB什么时候适合用 [https://www.mongodb.com/blog/post/an-introduction-to-change-streams]

Google Analytics cert on GCP (Coursera) free 7 days: https://google.qwiklabs.com/courses/905&utm_source=cloud-dot-google&utm_medium=website

https://towardsdatascience.com/https-medium-com-martin-weitzmann-bigquery-sql-on-nested-data-cf9589c105f4

NoSQL-ElasticSearch

Research new skills: https://druid.apache.org/docs/latest/development/extensions-core/datasketches-extension.html


Data integration:Kafka,Nifi. Data Wrangling:Lavastorm (COnsulting)
Mongo (document DB)might be a way to capture change, otherwise new columns/rename may break UI
## Selected interview records:
decimal
convert to date CAST(x=1 AS STRING)
datepart: EXTRACT( day/month FROM field)
Q1
daily balance (get each day each cust's last trans - considering 0 balance or no trans)
Q2.
get amount change of chosen customer (bonus Q)
Q3.
get each centres' percentage( maybe instead of cartesian, use sum over partition by)

### Gitlab (a remote company):

passed online screening (SQL questions and behaviour, purpose questions, no time limit);
didn't pass US remote HR lady round on question like "why you choose gitlab) (just 18 min video call and no further response)

Possible reasons: could be location? or culture fit

### Prospa

passed online ETL python test (time suggested 90 minutes) , did a code review regarding formatting, devops, pipeline
DW最重要3个与数据库区别 因columna 所以是:bulk loading, encoding, compression. 我说Sort Key Distribtion Key 
hot fix? On Prod I would have a planned script.他说直接改
incremental loading: 1. detect change using timestamp, compare value?3. deal with change dimension

Best practice of jupytor notebook.:我就说我写大的
How do you design 1 人偏啰嗦500 变量。不停小提交做trail.允许下游改code, 2 reviews.


### Toptal

Online SQL test with time limit, moderate difficulty

### freelancer

Online Python/SQL test with time limit

### 


weRemote:
 ETL processes in a variety of platforms (Matillion {required}, Pentaho, Microstrategy, Talend, CloverETL, FiveTran, Stitch)
 
 BI engineer:

    Traditional data warehouse skills - ETL / SSIS / Informatica /
    Strong SQL / data mapping / data migration experience
    Cloud technologies such - AWS / Azure / Big Insights
    Big data tech - Hadoop / Hive / Spark / etc
    Data integration tools - Talend / Informatica / Mulesoft
    Python / R  / NoSQL / MongoDB 

## tell fake data scientist

A few that I particularly like:
1) Explain a p-value
2) Explain how diversity reduces error and bias in ensemble methods
3) How do gradient boosting and bagging differ theoretically (and in deployment within a system)
4) Name and explain 3 different dimensionality reduction strategies
5) Explain boostrapping and its practical uses in machine learning
6) Explain the math behind PageRank and how linear algebra in general can be used on graph/network problems
7) How would you explain random forest to a kindergartener using the objects in this room
8) Explain one contribution of topology/geometry to the field of statistics and machine learning in detail
9) When is it not appropriate to use deep learning methods on a problem
10) Explain Bayes Theorem in layman's terms
11) Why is a control group necessary for testing
Those should cover a breadth of important topics and give an idea of a person's depth as a data scientist beyond knowing the basics behind buzz-words.
