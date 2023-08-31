### olist

changelog:
1. Initial commit
2. Added most of the data & context required to start exploring the dataset.


Brazilian E-Commerce Public Dataset by Olist:
```
olist_customers_dataset.csv
olist_geolocation_dataset.csv
olist_order_items_dataset.csv
olist_order_payments_dataset.csv
olist_order_reviews_dataset.csv
olist_orders_dataset.csv
olist_products_dataset.csv
olist_sellers_dataset.csv
product_category_name_translation.csv
```
Marketing Funnel by Olist
```
olist_closed_deals_dataset.csv
olist_marketing_qualified_leads_data
```
Joining with Brazilian E-Commerce Public Dataset by Olist
This dataset can also be linked to the Brazilian E-Commerce Public Dataset by Olist using seller_id. There you will find information of 100k orders, price, payment, freight performance, customer location, product attributes and finally reviews written by customers.

#### Joining both the datasets

https://www.kaggle.com/code/andresionek/joining-marketing-funnel-with-brazilian-e-commerce/notebook



#### Insights from others

R Code to generate the SQLite DB from main ECommerce dataset.

https://github.com/curso-r/basesCursoR

https://github.com/curso-r/basesCursoR/blob/master/data-raw/olist.R




Resolved issue with order_review text with commas. 

https://github.com/renanfmoises/olist-csv2postgres-etl/commit/c39852fc481a391c78ca06d52f1d2a4bbc72b987#diff-a151287aae155243a482366934ce7e26ef27db997968cd3757bcabde8f5c583a


correcting NULL values in orders table 

https://github.com/pauloreis-ds/olist-database-postgresql/commit/60736471e8e9ab6dc337e9d45b7dc13bd55c73e6

Mara Olist E-Commerce

https://github.com/mara/mara-olist-ecommerce-data/tree/master/olist_ecommerce

feat: sql commands to create DB in PostgreSQL usign pgAdmin4

https://github.com/JuanD13Perez/Olist_EDA/blob/main/queries/olist_db_creation.sql

-- Now that the data has been cleaned, we're ready to use it for our analysis!

https://github.com/akbarfithrawan/SQL-Project-Olist/blob/main/olist-data-preparation.sql

Making tables:

https://github.com/emso-exe/Comercio_eletronico_brasileiro/blob/main/scripts/script_00_criacao_bd_tabelas.sql

Geo Brazil for geospatial

https://github.com/KurtHeld23/geo_Brazil

#### Articles

Olist analysis with SQLite

https://www.kaggle.com/code/alexanderershov/olist-analysis-with-sqlite

Ecommurz’ sales performance: Data wrangling with the Olist database

https://medium.com/@lingostat/ecommurz-sales-performance-data-wrangling-with-the-olist-database-8c0ad43e2eb2

Exploring Olist Ecommerce Dataset

https://blog.devgenius.io/exploring-olist-ecommerce-dataset-59652562496d

SQL and analytics

https://leewtai.github.io/courses/stat_computing/lectures/python_mds/sql.html

#### JOB INTERVIEW
# Data Analytics

https://github.com/olist/work-at-olist-data

# Practice test (work-at-olist-data)

This is the page about the practical test for candidates for the selection process of data scientists, analysts and engineers for olist's Business Science & Analytics team.

## Getting to know our data team:
[BSA: a team of people who go beyond tools and numbers](https://medium.com/olist/bsa-um-time-de-pessoas-que-v%C3%A3o-al%C3%A9m-das-ferramentas-e-n%C3%BAmeros-76a073cadd67)

## Scenario

Olist is the largest department store on marketplaces. It has a catalog with over 950,000 products, hundreds of thousands of orders and a network of over 9,000 partner retailers spread across all regions of Brazil. We understand that the data and intelligence area is one of the main drivers of business growth, which is why we are looking for professionals passionate about data to join our Business Science and Analytics (BSA) team.

We're constantly generating data, data, and more data. Our scenario is big data!

## How is our database?

Consider that the figure below is the structure of our e-commerce database and that each table in this database is available as a dataset. [Here are the datasets](/datasets). Note that the data are sample and are presented in the relational model, as they were extracted directly, without any treatment, from the transactional environment.

![Database Structure](images/schema.png)
Well, here you can see how a product is displayed on the e-commerce platform.

![Example of product displayed on the platform](images/example.png)

## Challenge

This e-commerce platform transacts Brazilian retail data. Therefore, the company's business areas face some doubts and challenges, such as:

* Can our different associated retailers maintain the same price for the same product without major discrepancies?
* Can we give the same benefits to all retailers (sellers)? Or are there any that stand out?
* Is there a difference in shipping costs in different regions/cities? Or can we apply the same freight subsidy rules to any location?
* Is our product catalog comprehensive? Or does it focus on specific categories?
* Do we always sell the same products? Or are there seasonalities?
* Is there a predictive model to prepare us for the future?
* Will the current database support our growth? Or is there a more scalable option?

He was confused. Below are more specific tips for each role.

### Data scientist
* How about a textual analysis of customers who left reviews about their purchases?
* Some customers did not write a review. But why are they satisfied?
* With purchase date information, you will be able to predict future sales!
* You will also be able to focus on logistics and find ways to optimize delivery times.
* This data has geolocation coordinates. Are there differences in consumption patterns by region?
* Have fun discovering the product categories most prone to customer dissatisfaction.
* Create features from this rich dataset, feature engineering, or attach some external public information to it.
* And a model for pricing the products in our catalogue? Mathematical modeling to optimize routes? Hypothesis tests to validate any question?
* How about writing a report or slides detailing your findings?
* Feel free to create your own approach if you consider that the previous tips are not relevant.

### Data Analyst and Business Intelligence
* Think of some KPIs for monitoring. Perhaps others for managers to direct!
* Cross-referencing the data could generate interesting reports. After all, who are the Top 10 in sales? What kind of products do they sell? What is their impact on the business?
* How about carrying out an exploratory data analysis. And then? Does something catch your attention?
* You could present this data in a dashboard. This would speed up decision-making!
* We are interested in your skills with applied mathematics and descriptive statistics. What can you show us with the data?
* How about writing a report or slides detailing your findings?
* Feel free to create your own approach if you consider that the previous tips are not relevant.

### Data engineer
* We would like to analyze your skills with SQL, dimensional modeling and data integration. Show your knowledge of ETL processes and Data Warehouse concepts. How about replicating our datasets, remodeling them into a database and presenting the improvements made in their creation.
* Is it possible to use the proposed model in a cloud environment? What platforms or services would you use? What are the advantages of the chosen model in terms of performance?
* Some team members say that the current database modeling is suitable for use by data scientists and BI analysts, however, others say that there are ways of modeling databases that will bring more efficiency. What is your opinion on this?
* Are we concerned about the skyrocketing volume in our current database? Would you consider a more scalable option or should we maintain the existing structure?
* Our dashboard visualization tool is slow and our team has detected that the problem is in the data infrastructure. How would you approach this situation from a data architecture point of view?
* Our database is hosted in the cloud and our data analysis tools are "on premises". Would you keep this arrangement or make changes for more performance?
* Our operational area needs real-time information, but the company's directors, who only monitor information on monthly KPIs, claim that this is unnecessary and would result in costs. What is your position on this?
* Our team that is focused on Data Governance claims that documenting processes is more important than refactoring the more than 500 scripts that are running slowly. How would you act in this impasse, if you had to prioritize work?
* Here at olist, we are very hands-on! As a Data Engineer, show us what you can do in practice with our database. (We know it's a sample, but imagine the whole could be petabytes of data)
* How about writing a report or slides about your approach to solving some of these problems?
* Feel free to come up with your own approach if you feel that the previous tips are not relevant.

## What do we expect from the candidate?

We want to understand your technical proficiency, analytical reasoning and presentation of results.

**You don't need to answer all the questions or tips listed above, they are just suggestions (keep the focus on what you are most interested in).** However, we want to have a clear perception of how you solve problems.

For this, feel free to adopt software, processes and tools that you consider appropriate.

You will have a period of up to 7 days and after completing the test, send us a report contextualizing the work carried out and your solutions. It can be in any format, we just want to understand how you present the results of your work.

Do not forget to indicate in your report the links/addresses, if you have hosted codes/files in any repository on the internet.







# Marketing Analytics

https://github.com/olist/work-at-olist-marketing

# Work at Olist - Marketing Analytics
*Apply for a job at Olist's Marketing Analytics Team: http://bit.ly/work-at-olist-marketing*

[Olist](https://olist.com/) is the largest department store of Brazilian marketplaces. We connect small businesses to channels without hassle and with a single contract. We have connected more than 4.1 thousand sellers to stores like Americanas.com, Ponto Frio, Walmart, Submarino, Mercado Livre, Amazon, among others.

## Marketing Analytics Team
Responsible for taking advantage of growth opportunitties, this team work close to data to create new lead capture tools, prediction models and advanced analysis.

This repository contains instructions to solve problems that are used to evaluate the candidate skills. It's important to notice that satisfactorily solving this test it is just a part of what will be evaluated. We also consider other disciplines like the capability of extracting insights from data, business understanding, data visualization skills, documentation and design.

## How to participate

1. Follow the instructions of README.md (this file);
2. Download the [test data available on Kaggle](https://www.kaggle.com/olistbr/marketing-funnel-olist/home). You may want to solve the problem online using Kaggle Kernels. 
3. Take your time to read carefully the data documentation and understand how it works. If you have any questions about the data, open a public discussion on the dataset page. 
4. Use the tool you like the most or are more familiar with to analyse the data and solve the problem:
   * [Kaggle Kernels](https://www.kaggle.com/kernels) for Jupyter Notebooks (Python/R);
   * [Colaboratory](https://colab.research.google.com) for Jupyter Notebooks (Python/R);
   * Google Sheets;
   * Microsoft Excel;
   * BI tools (Power BI, Tableau, Qlik, etc);
   * Any other tool you like;
5. Apply for the position at our [career page](http://bit.ly/work-at-olist-marketing).
6. Send your analysis by email (you'll get the address at the selection process).
7. You might be asked to explain some steps of your analysis at the interview.

> Completing the test and applying for the postion does not guarantee that you will be called for interview.

# Work at Olist Marketing Analytics - Test
## Dataset
Olist has released a [Marketing Funnel Dataset](https://www.kaggle.com/olistbr/marketing-funnel-olist/home) from sellers that filled-in requests of contact to sell their products on Olist Store. The dataset has information of 8k Marketing Qualified Leads (MQLs) that requested contact between Jun. 1st 2017 and Jun 1st 2018. They were randomly sampled from the total of MQLs.

This is real data, it has been anonymized and sampled from the original dataset.

## Requirements
You may want to solve different types of problems with this dataset. Choose one that best suits you and have fun! Bellow are some examples of things you might want to do, but feel free to use your creativity.

> Notice that you **are not required to do everything** listed bellow. Those are just starting points, ideas to guide your work. Remember that quality is more important than quantity.

**Language Requirements:** We like to experiment new things! Feel encouraged to solve the test with a tool you like the most. We accept solutions on spreadsheets or presentations in pdf. But you are really going to touch our hearts if choose tools like Python/R to solve this problem. Showing your code/solution is a plus.

### Aquisition Channels
* Analyse the performance/results of our aquisition channels through the marketing funnel
* Link the data with the orders dataset and estimate the customer value for each channel
* Create KPIs and a dashboard that shows the current funnel status and provide some insights
* Find some opportunities to improve the area by using data. Which channels should we invest more? Wich ones should we stop?
* Find correlations between data and try to predict an outcome (closing a sale, for instance)

### Engineering Marketing
* Develop a plan to attract and capture more qualified leads (tool based marketing)
* Propose some tests to analyse and improve our performance

> **Or just tell us something we don't know. Which business value would you create for Olist with this data?**

# General SOftware Assignement: Create a web app for authors

# Work at Olist

[Olist](https://olist.com/) is a company that offers an integration platform for sellers and marketplaces allowing them to sell their products across multiple channels.

The Olist development team consists of developers who love what they do. Our agile development processes and our search for the best development practices provide a great environment for professionals who like to create quality software in good company.

We are always looking for good programmers who love to improve their work. We give preference to small teams with qualified professionals over large teams with average professionals.

This repository contains a problem used to evaluate candidate skills. It's important to notice that satisfactorily solving the problem is just a part of what will be evaluated. We also consider other programming disciplines like documentation, testing, commit timeline, design and coding best practices.

Hints:

* Carefully read the specification to understand all the problem and artifact requirements before starting, if you don't understand something tell us;
* Check the recommendations and reference material at the end of this specification;
* We appreciate simplicity, so create a good project setup that will help us in your evaluation;
* Please make tests ... we appreciate tests <3... tests make the world better.

## How to participate

1. Make a fork of this repository on Github. If you can't create a public fork of this project, make a private repository (bitbucket/gitlab/github offers free private repos) and add read permission for one of these users below:
    * [tech-hiring on github](https://github.com/tech-hiring);
    * [tech-hiring on bitbucket](https://bitbucket.org/tech-hiring);
    * [tech-hiring on gitlab](https://gitlab.com/tech-hiring).
2. Follow the instructions of README.md (this file);
3. Deploy your project on a hosting service (we recommend [Heroku](https://heroku.com));
4. Apply for the position at our [career page](https://olist.gupy.io/) with:
    * Link to the fork on Github (or bitbucket/gitlab);
    * Link to the deployed project in a hosting service.

## Specification

You should implement an application for a library to store book and authors data.

**This application must provide an HTTP REST API to attend the requirements.**

### 1. Receive a CSV with authors and import to database

Given a CSV file with many authors (more than a million), you need to build a command to import the data into the database. The CSV file will have the following format:

```
name
Luciano Ramalho
Osvaldo Santana Neto
David Beazley
Chetan Giridhar
Brian K. Jones
J.K Rowling
```

Each author record in the database must have the following fields:

* id (self-generated)
* name

You need to store the authors' data to complement the book data that will be stored afterward (see item #3).

_Extra tip: If you use Django Framework you can do something like this..._

```
python manage.py import_authors authors.csv
```

### 2. Expose authors' data in an endpoint

This endpoint needs to return a paginated list with the authors' data. Optionally the authors can be searched by name.

### 3. CRUD (Create, Read, Update and Delete) of books

You need to implement these actions in your API:

* Create a book
* Read book's data
* Update book's data
* Delete book's data

Each book record has the fields:

* id (self-generated)
* name
* edition
* publication_year
* authors (more than one author can write a book)

To retrieve a book (in easy mode) we can filter by 4 fields (or a composition of these four):

* name
* publication_year
* edition
* author

But these 4 filters are optional. It must be possible to navigate all the books' data without any filter.

To create a book you need to send this payload (in json format) below:

```
{
 "name": // Name of the book;
 "edition": // Edition number;
 "publication_year": // Publication year of the book;
 "authors": // List of author ids, same ids of previous imported data
}
```

## Project Requirements:

* Provide a working environment with your project (eg. Heroku)
* Application must be written in Python or Go.
* Python
    * Use Python >= 3.5
    * Choose any Python web framework you want to solve the problem
    * Use PEP-8 for code style
    * [Python Coding Style](http://docs.python-guide.org/en/latest/writing/style/)
* Go
    * Go >= 1.10
    * [Effective Go](https://golang.org/doc/effective_go.html)
* Every text or code must be in English
* Write the project documentation containing:
    * Description;
    * Installing (setup) and testing instructions;
    * If you provide a [docker](https://www.docker.com/) solution for setup, ensure it works without docker too.
    * Brief description of the work environment used to run this project (Computer/operating system, text editor/IDE, libraries, etc).
* Provide API documentation (in English);
* Variables, code and strings must be all in English.

## Recommendations

* Write tests! Please make tests ... we appreciate tests <3... tests make the world better;
* Practice the [12 Factor-App](http://12factor.net) concepts;
* Use [SOLID](https://en.wikipedia.org/wiki/SOLID_(object-oriented_design)) design principles;
* Use programming good practices;
* Use [git best practices](https://www.git-tower.com/learn/git/ebook/en/command-line/appendix/best-practices), with clear messages (written in English);
* Be aware when modeling the database;
* Be careful with REST API details. They can bite you!

**Have fun!**
