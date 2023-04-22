# data-analysis-work
Data analyses related to various fields such as Health, Retail, Finance, HR and so on are compiled here

**PROJECT 1: COVID 19 DATA ANALYSIS**
## Data sources
- **Confirmed cases and deaths:** this data is collected from the [World Health Organization Coronavirus Dashboard](https://covid19.who.int/data). The cases & deaths dataset is updated daily.
COVID 19 dataset is available in [CSV](https://covid.ourworldindata.org/data/owid-covid-data.csv)


                                   
| Variable                     | Description                                                                                                                                                                                                                                |
|:-----------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `continent`                  | Continent of the geographical location                                                                                                                                                                                                     |
| `location`                   | Geographical location                                                                                                                                                                                                                      |
| `date`                       | Date of observation                                                                                                                                                                                                                        |
| `median_age`                 | Median age of the population, UN projection for 2020                                                                                                                                                                                       |                                                                 
| `total_cases`                    | Total confirmed cases of COVID-19. Counts can include probable cases, where reported.                                                                                                                  |
| `new_cases`                      | New confirmed cases of COVID-19. Counts can include probable cases, where reported. In rare cases where our source reports a negative daily change due to a data correction, we set this metric to NA. |
| `total_deaths`                    | Total deaths attributed to COVID-19. Counts can include probable deaths, where reported.                                                                                                                  |                                                      

**Ask:**
1. Find the total number of cases, deaths, new cases
2. Compare Total death by Continents
3. Compare median age by Continent and top 5 countries
4. Compare total cases by Country( Top 10 countries by total number of cases
5. Compare Total cases by year and country ( Top 5)

**Prepare:**
Dataset is loaded from Excel sheet and imported into Power BI 

**Process:**
Data cleaning is done by Transform data in Power Query Editor by :
1. Removing columns other than the variable columns that are mentioned above in Power BI 
2. Columns are renamed for better labeling by removing underscores and using ProperCase

**Analyze:**
Trends are analyzed 
1. Continent vs deaths
  
    Europe and South America has highest number of deaths while Oceania Continent has lowest number of deaths

2. Continent vs new cases
  
    Asia has highest number of new cases and Oceania has lowest number of new cases

3.  Median Age vs Top 10 countries
    
    France has highest average median age which is, 42.00 and India has lowest average median age of 28.20

4. Total cases vs Country
    
    Total cases are highest in U.S. and lowest in Italy



----

**PROJECT 2: BRIDGING COMMUNICATION GAP BETWEEN TEACHERS AND PARENTS**

Possible Solution: DESIGN AN APP FOR PARENTS TO STAY UPDATED ON SCHOOL NEWS , CHILDEREN'S CLASSES AND ACTIVITIES

**Ask:**
1. Why do we want to design an app and why we want to keep parents informed?: Quantity impact on student test scores
2. How to identify what parents want to know about 
    
WHY? 
There are two factors contributing towards it:
1. Downward trend(data taken from 2008 -2012, scores falling from 2008 to 2022)
2. Parent involvement also dropped >10% from 2008-2022
   Thats why parental invovement is required to improve student test scores
    
HOW? 
1. Data taken from survey and dividing it in 3 groups:SPORTS, ACADEMICS, EXTRACURRICULAR
2. Check the current trend for 6th ,7th and 8th Graders=> Here I found least attention is given to 8th and they are getting least news alerts.
    PRIORITIZE 8th Graders
 
 Lets design app with 3 tabs for each of the category and do test launch on parents of 8th Graders
 
**Analyze**    
1. WHY: Parental involvement correlated with higher test scores
2. HOW: Creating an app with 3 gtabs for each category and doing test of version 1 of app on the parents of least involved group( which was 8th graders here)
    
**Further Exploration**
1. Impact if multiple children are enrolled in same school
2. Impact of single vs multiple caretaker


----

**PROJECT 3: BIKE SHARING ANALYSIS TO CONVERT CASUAL RIDERS TO ANNUAL MEMMBERS FOR SPEEDY SUCCESS**
  
  **OBJECTIVE:**
  
  In this case study, I am a “Jr. Data Analyst” at a company called Cyclistic, a bike sharing company based in Toronto.
  
  The bikes can be unlocked from one station and  returned to any other station in the system anytime. 
  
  Cyclistic, offers both Classic and Electrical bikes to annual members and casual riders. 
  
  Members are defined as users who have annual passes. Casuals, on the other hand, refers to users who have purchased either a single day pass or a day pass.
  
  Finance team of the company has come to conclusion that annual members are more profitable than casual riders.

**Ask:**
1. How do annual members and casual riders use bikes differently?
2. Why would casual rider turn into annual member?
3. How to use digital media and influence them for conversion?
  
  To answer 1st question, I will prepare and process last 13 month data
  
**Prepare:**
1. All personal information of riders (e.g. regarding purchases to determine whether they live near Cyclist service location or whether they have multiple single passses), is removed for security purposes
2. Docked bikes and classic bikes refer to same thing
3. Trips' time contraints are kept in between 1 min and 1 day. Rides not within these constraints are maintenance or stolen
4. Additional column named" ride_length" is created by difference between started_at and ended_at in time format "HH:MM:SS"
5. Another column for determining day of week is also created
6. Any empty rows are deleted as first step and then start looking for duplicate data, and at last check for 1 to 5 points
 
**Data Source:**
                                   
| Variable                     | Description                                                                                                                                                                                                                                |
|:-----------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| `ride_id`                  | Unique bike trips.                                                                                                                                                                                                     |
| `rideable_type`                   | Three different types of bikes: classic, docked, electric.                                                                                                                                                                                                                     |
| `started_at`                       | Date and time that bikes started at stations.                                                                                                                                                                                       |     
| `ended_at`                 | Date and time that bikes ended at stations.                                                                                                                                                                                                 |                                                               
| `start_station_name`                    | Name of station from where ride started.                                                                                                                                                                                       |     
| `start_station_id`                      | ID of station from where ride started.                                                                                                                                                                                                                       |
| `end_station_name`                    | Name of station from where ride ended.                                                                                                                                     |
| `end_station_id`                  | ID of station from where ride ended.                                                                                                                                           
| `start_lat`                   | Latitude of starting point of ride.                                                                                                                                                  |   
| `start_lng`                       | Longitude of starting point of ride.                                                                                                                                            |
| `end_lat`                 | Latitude of ending point of ride.                                                                                                                                                         |                         
| `end_lng`                    | Longitude of ending point of ride.                                                                                                                                                        | 
| `member_casual`                      | Annual or casual riders.|     
  	
