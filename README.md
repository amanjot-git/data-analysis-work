# data-analysis-work
Data analyses related to various fields such as Health, Retail, Finance, HR and so on are compiled here

**PROJECT 1: COVID 19 DATA ANALYSIS**

**Source: Power BI Projects by The Machine Learning on Udemy**

**Data sources:**
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

**Source: Google Data Analytics Professional Certificate**

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
  **Source: Google Data Analytics Professional Certificate**
  **OBJECTIVE:**
  
  In this case study, I am a “Jr. Data Analyst” at a company called Cyclistic, a bike sharing company based in Toronto.
  
  The bikes can be unlocked from one station and  returned to any other station in the system anytime. 
  
  A bike-share program that features more than 5,800 bicycles and 600 docking stations.
  
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

**Some errors to check for:**
1. started_at/ended_at: There are some values in these columns where rides dont follow the constraint i.e <1 min or >24 hours.
2. start_station_name/end_station_name: Inconsistencies in these columns are spaces, null value, missing a start and end station name because electrical bikes have the option to lock and unlock near at a station. But starting and ending station names shouldnt be  missing from classic bikes, and as there are certain data where it happens, then such records need to be removed. Classic bikes must have a start and end station name.
3. start_station_id/end_station_id: Inconsistencies are present with the column.They dont add any value to our analysis.
4. start_lat/end_lat & start_lng/end_lng: these columns refer to starting and ending longitude and latitude for the bike. This data will be later used for data visualization.
5. member_casual: these columns refer to either annual or casual riders. These are the only two values allowed in the column and was double checked for errors.
  	
Data Cleaning process:
1. Replaced 'docked_bike with 'classic_bike'
2. Removed trips where null was in start or end station of classic bike , and latitude or longitude columns are null
3. Replaced null values in the station name columns with the string `On Bike Lock` for only electric bikes.
4. Cleaned up station_name from spaces at front or trail
5. ride_length and day_of_week for trip is calculated
6. Removed trips where the ride time length was less than or equal to 1 minute and greater than or equal to 1 day.
Removed trips that contained the word “REPAIR” on station names.
In total, I removed about 138K rows to be left with a clean combined table with about 5.5 million rows.


![image](https://user-images.githubusercontent.com/59747572/235278621-f10869cf-63e3-457f-81c3-21481112ff7d.png)

Uploaded all clean files to Google Bigquery 

Created a combined table using UNION ALL on all tables and added columns Year, Month, DayofWeek, Formatted ride_length for comparison

**ANALYSIS OF MEMBER AND CASUAL RIDERS ANALYSIS OVER MONTH AND DAY OF WEEK**

![image](https://user-images.githubusercontent.com/59747572/235314354-885447e6-f6ab-435c-90c7-5d711e3cd8a1.png)






![image](https://user-images.githubusercontent.com/59747572/235334573-ef06fde3-a826-4170-b666-afa5ab41b363.png)





From the results, it is evident that
1. The number of casual riders as well as members increase as the weather becomes warm and starts to go down as fall season approaches. 
2. Members ride mostly during weekdays.



**PROJECT 4: Manufacturing Oil Rig Prompt - Avery Smith**

Source: Dataset comes from a real hydraulic rig system. This hydraulic rig is used to drill oil out of the ground.
It has 4 main controls: the cooler setting,the valve setting, the pump setting, and the accumulator setting. The rig has sensors in different areas measuring the pressure, volumetric flows , and temperatures.
I am tasked with creating a manufacturing monitoring dashboard that allows management to understand the manufacturing process in detail

**Data Sorces:https://raw.githubusercontent.com/AveryData/hp-pred/main/HourlyData.csv **




