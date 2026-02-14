# insights-sales


Name: Ruchi Mali
Email: ruchim2109@gmail.com

Role: Data Science / Applied AI Engineer
Submission Format: GitHub repository + README
________________________________________
Section 1 
1.	What do you think is the real business problem here?
The real business problem , is to understand the metadata of deals, rather based on the current or past deals undertaken where what and how things are affected and consequently the results are changed, understanding this can we take insights and change startergies when in some aspects arising later, meaning any business works on certain metrics or has way of working this working as time proceeds and company progresses from their data which holds very useful and important insights these insights can be helpful in changing the course if business fails to meet expectations, or deadlines, with those insights what can be made better can be changed can be made unique and implemented, also how well the prediction of ceratin startergy may behave can be tested, the problem here is fundamentally I have my business data and way of working how  can it be used to identify and make my workflow better and eventually help me in achieving progress in the business by implementing smart decisions to maximize the business potentias
2.	What key questions should an AI system answer for the CRO?
Must answer all fundamentals questions with why how what 
1.	Why a strategy will fail
2.	What factors affect the revenue or win rate or positive progress
3.	How will the current strategy be improvised
4.	How will the next quarter be improved based on current patterns trends analysis and insights 
5.	Why is loss occurring what factors need to be taken care of 
6.	Where is the business lacking what are the opportunities alternative and best solution to avoid or reduce the 
7.	How change can be made to maximize profit and minimize loss with support of predictions with certain accuracy and support 
8.	If a strategy is implemented what are he supporting factors and the performance predictions 
9.	What is the best path 
3.	What metrics matter most for diagnosing win rate issues?
It would be 
1.	targeting product to proper region and industry meaning a product of a particular region or industry may result in more win rate , relation of product to region industry 
2.	Representative dealing out a deal , how are they abke to success in a type of deal an the customer too , representative to product and region or industy relevance/ dpeendecy and win rate too 
3.	Deal closing time how much time it took for the deal to actually cloe show 
4.	Deal amount and closing interval dependency 
5.	Which industry deals are closed more often and at what rates same for region and products 
6.	Which lead source is effective for a product / region or industry and its corresponding win loss issue 
4.	What assumptions are you making about the data or business?
1.	The data is complete and useful for getting actual actionable insights meaning not demo with no patterns 
2.	Closed deals carry real value, meaning the deals won really depict the true nature of how the deal was done not dummy values
3.	Each row consist of unique deals leading to unique conclusion
4.	No fundamental business model is changed because that would directly in fluence deals undertaken in a period and hence their behaviour leading to wrong conclusions 
5.	Open deals are also been really undertaken not dummy values
6.	Deal stages are updated properly not abandoned or wrongly answered  

Section 2 - EDA
Please see the goggle colab file has the eda properly done wih conclusion and analysis 
Identify at least:
o	3 meaningful business insights

o	The insights I found are as follows 
o	1.Core products are more closed in APAC
Why does it matter?
Focus on what kind of products in what region, and focus son more such delas wuie potentials 
o	What action could it drive?
Focus on more such deals, which region what typw of product need  to be concentrated on 
2. All representatives seem to have equivalent win loss ratios 
o	Why does it matter?
Whether to improve staff training more representatives 
o	What action could it drive?
o	Start training of representatives give focalized ares to representative etcs 
o	
3. less pro deals are from parterner and more from other sources
Why matter
Know which source can be can be used for ehta kind of deals 
What action
 Use that type of source for more of those deals 
o	2 custom metrics you invent yourself (not just standard ones)

o	Pipeline concentration – menaing  is pieline concentrated on particular aspect like concnetentaretd only on few factors analyses that with this factor 

o	Deal velocity means deal outcomes done in what cycle divided by state of the deal in numerical weightage like propersed etc says how fast the deal is done by weighatyge 


Section 3 
Option B – Win Rate Driver Analysis
Identify which factors are hurting or improving win rate.
•	Define the problem clearly
The problem states to find out all the possible reasons or fctors which either hurt ior improve the win rate example a particular region deals are improving win rates, or a acombination of region produt type deal closing time improves or decreases the win rate, the wirn rate factor ananl;ysis will help rto fdentify factors which can affect the win closing of deals and hence improvement startegries or changes in the workflow or deals can be done meaning factors strongly contribvutinfg to winning deals can be used more often concentrated on or can be usedfor fture deals to make more successful deals and stratergies to reduce the win loss rate meaning favtors really disturbing the win rate like may be industry or representatice can be improved with searching for potiential clients or industries and training etc 
•	Build a simple model or rule-based system
done
•	Generate actionable outputs
•	Explain how a sales leader would use this
Using this factors or analysis the sales leaders can implement new stratergies example like if a product deals are winning less than can focus on typical products where deals are better or for failing products what factor fails , and correct or improve it like representative training imporiving locating and connecting to potential industries, products or regions which can help in closing deals that are successful for instance pro deals are done in india more successfully follow for more potential clients for pro deals, or expalnd market for other enterprise deals or other product or industries, they can also use the data to have prediction on an goinoing deal whether it will close or no how much more effort it will require like if a deal isfrom a lead source in a country it make close so proper folloup and other efforts can be implemented, focusing on a particular lead source, prediction whether an ongoing deal has been fop so many days and at such state andsuch deals had rthis wing rate in past compare  current factirs datat with old and see if more efforts need to vbe done as deal will close or no or focus on other deals like give more importance to deals an implement strategy , if a deal with huge amount can be closed in a specific region.


Section 4 and 5 
•	Architecture 
1.	CRM (Salesforce / HubSpot)
2.	Data Ingestion Layer (API / Batch Pull)
3.	Data Warehouse (Snowflake / BigQuery)
4.	Feature Engineering Layer
5.	ML Engine (Risk Model + Driver Model)
6.	Insights Engine
        │
        ├── Dashboard (BI Tool)
        ├── Slack Alerts
        └── Email Alerts
•	Data flow
1.	CRM updates deal
2.	Data ingestion pulls updates
3.	New data stored in warehouse
4.	Feature pipeline updates features
5.	Model scores all open deals
6.	Alert rules evaluated
7.	Alerts sent to Slack / Email
8.	Dashboard refreshed
•	
Lightweight Sales Insight and Alert System
•	High level architecture
•	Data sources include CRM system, payment gateway, deal management tool, and marketing platform
•	Data ingestion layer pulls data using APIs or scheduled batch jobs
•	Processing layer performs cleaning, aggregation, KPI calculation, and anomaly detection
•	Business logic layer generates insights and alert conditions
•	Storage layer includes a structured database for processed data and a lightweight cache for recent metrics
•	Alerting layer sends notifications through email, Slack, or dashboard updates
•	Dashboard layer provides visual reporting for sales managers and leadership
•	Data flow
•	Raw sales and deal data is extracted from source systems daily or hourly
•	Data is validated for missing fields, incorrect formats, and duplicates
•	Cleaned data is stored in a central database
•	KPI engine calculates metrics such as total revenue, average deal size, conversion rate, and sales cycle duration
•	Anomaly detection module compares current metrics with historical baselines
•	If thresholds are breached, alert rules are triggered
•	Alerts are sent to relevant stakeholders and logged for tracking
•	Dashboard is refreshed with the latest insights
•	Example alerts or insights
•	Revenue dropped more than 20 percent compared to last week
•	Conversion rate declined significantly for a specific region
•	Average deal size increased above historical average
•	Large enterprise deal stuck in negotiation for more than 30 days
•	Unusual spike in discount percentage applied by a specific sales rep
•	Monthly target likely to be missed based on current pipeline velocity
•	How often it runs
•	Data ingestion runs hourly for near real-time tracking
•	KPI computation runs every hour or daily depending on business need
•	Alerts are evaluated immediately after each processing cycle
•	Weekly summary reports are generated automatically
•	Monthly executive summary is generated at month end
•	Failure cases and limitations
•	Data source API failures may cause missing or delayed insights
•	Inconsistent CRM data entry can distort metrics
•	Fixed threshold rules may generate false positives
•	System may not capture qualitative reasons behind performance drops
•	Scaling issues may occur if data volume grows rapidly
•	Alerts may be ignored if too frequent, leading to alert fatigue
•	If SkyGeni were to productize this
•	Offer it as a modular SaaS product integrated with common CRM systems
•	Provide configurable alert rules and custom KPI definitions
•	Include AI based predictive forecasting models
•	Offer role based dashboards for sales reps, managers, and executives
•	Include audit logging and explainability for alerts
•	Provide enterprise security, access control, and compliance features
•	Offer API access for integration with other enterprise systems

Section 5 – Reflection
•	Weakest assumptions
•	Assumed that CRM data is clean and consistently structured
•	Assumed historical patterns are stable enough for anomaly comparison
•	Assumed alert thresholds are universally applicable across teams
•	Assumed user adoption of alerts and dashboards will be high
•	What would break in real world production
•	Poor data hygiene would reduce trust in insights
•	Edge cases such as seasonality or market shocks may trigger misleading alerts
•	High scale data could cause performance bottlenecks
•	Integration changes in third party APIs could disrupt ingestion
•	Alert fatigue may reduce system effectiveness
•	What would I build next if given one month
•	Replace rule based alerts with machine learning anomaly detection
•	Build forecasting models for revenue and pipeline prediction
•	Add explainable AI layer to justify why alerts were triggered
•	Introduce user feedback loop to improve alert quality
•	Add benchmarking across regions and teams
•	Improve data validation and automated data quality monitoring
•	Part of the solution I am least confident about
•	Threshold based anomaly detection accuracy
•	Handling incomplete or inconsistent data
•	Long term scalability without redesigning architecture
•	Adoption and behavioral response from sales teams
•	Predictive accuracy without sufficient historical data

