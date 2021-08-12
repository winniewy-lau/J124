# J124 Data Journalism Final Project: California Wildfires 2013-2019 
By Winnie Lau, Journalism student at the University of California Berkeley 

Data: 2013-2019 California wildfires dataset from California Department of Forestry and Fire Protection (Cal Fire)

## Part 1. Story Summary and Sourcing</summary>

### Data Analysis Summary (More detailed analysis process in Part 3)

**Number of wildfire**

The wildfires were concentrated in Riverside and San Diego counties in Southern California and Butte county in Northern California. The number of wildfires has increased 2.7 times from 162 in 2013 to 438 in 2017 and then dropped to 266 in 2019. 

**Severeness of Wildfires**

The size of wildfire fluctuated between 450 thousands to 600 thousands acres in 2013-2016 and significantly increased to 1.7 million in 2017 and even 3.4 million acres in 2018. It dropped to 280 thousand acres in 2019. The top 3 counties with the largest acres burned are Lake, Mendocino, and Trinity near the Northern California Coast. The top 3 deadliest wildifires occurred in Northern California in 2017 and 2018 -- Camp Fire (2018) in Butte County, Tubbs Fire (2017) in Napa and Sonoma counties, and Redwood Valley Fire (2017) in Mendocino county. Camp Fire remains the deadliest wildfire in California's history. 

**Timing**

The data also shows that there is a trend of wildfires starting later than previous years. 

### Story Idea

Based on the findings, we see a trend of increaing number and severeness of wildfires. This data story will be about the trend of California wildfire and the atmospheric and geogrphical factors affecting the scale and severeness of the wildfires. In particular, the story will focus on the relationship between climate change and the severeness of wildfire. 

### Story Sourcing

I would interview CalFire Northern Region Chief,	Mike Bradley, (530) 224-2460, and CalFire Southern Region Chief,	Dave Fulcher,	 (559) 243-4127 for their comments on the wildfire trend. I would also interview experts in wildfires, for example, UCLA Climate scientist, Daniel Swain, PhD, (dlswain@ucla.edu). He studies how the atmospheric phenomena increases the risk of severe wildfires. His insight would add the relationship between climate change and wildfire to the story. I would also interview UC Davis Department of Public Health Sciences Professor Irva Hertz-Picciotto (ihp@ucdavis.edu). She studies the potential health impacts of wildfire, smoke and ash. She would add the impact of wildfires to the story. 

Regarding additional sources, I would use the statistics of wildfires on CalFire website (https://www.fire.ca.gov/stats-events/), because it tells us the most updated statisitics, including the fires in 2020 and 2021. I would also use the report on "Top 20 Largest California Wildfires" by CalFire (https://www.fire.ca.gov/media/4jandlhh/top20_acres.pdf), because it tells us the trend of more severe wildfire in California. The report shows that five out of the top 6 largest California Wildfires occurred in 2020 and 2021. The acres burned by the August Complex in 2020 and Dixie Fire in 2021 have surpassed the Mendocino Complex in 2018 which was the largest wildifre in 2013-2019,

## Part 2. Data Visualization

<img src="https://user-images.githubusercontent.com/69986804/129123310-dac63066-73b5-4020-b49a-d8b41b30c75b.png" width=50% height=50%><img src="https://user-images.githubusercontent.com/69986804/129134117-4c2f223f-62fa-4357-82a4-c053f1ceece1.png" width=50% height=50%>

Link: https://www.datawrapper.de/_/EKQT7/

Link: https://www.datawrapper.de/_/DbONi/

## Part 3. Data Analysis Process

**Step 1: Download the cvs file dataset from https://www.kaggle.com/ananthu017/california-wildfire-incidents-20132020.**

**Step 2: Import the cvs file into Google Drive and open it as Google Form.**

Link to the original dataset and analysis in Google Form: https://docs.google.com/spreadsheets/d/1rnnjETdAG5IrVzZyMy7MB_zTS0gO9lA4MQA07RFwrDk/edit?usp=sharing

**Step 3: Look up unclear terms**
- What does "Major incidents" represent? 
  - Major emergency incidents could include large, extended-day wildfires (10 acres or greater), according to Cal Fire. 

**Step 4: Clean the dataset**
  - freeze and bold the first row
  - look for error or anomalies

**Step 5: Think of questions for the dataset, analyze the data and find the answers**

<details>
  <summary> Question 1. How many wildfire in total in 2013-2019? What are the top 5 counties with the highest number of wildfire? </summary>
    <br>
  
    1.1 Create a pivot table, choose "Counties" as the rows, and add COUNTA "CalFireincident" as Values.
  <img src="https://user-images.githubusercontent.com/69986804/128896978-96dc59e9-9083-4c7a-9951-2656dd5b029c.png" width=50%, height=50%>

    1.2 Copy and paste the result into a new tab. Add column titles "County" and "# WildFire". Freeze and bold the titles. 
    1.3 Sort the "# WildFire" column descendingly.
  **Result:** 
  - 1636 wildfire occurred in 2013-2019.

 <img width="220" alt="Screen Shot 2021-07-26 at 11 35 26 AM" src="https://user-images.githubusercontent.com/69986804/127040763-3c4f3f79-d91e-4863-bb25-bfe15a958cd5.png">

</details>
    
<details>
  <summary>
    Question 2. How many major wildfire in 2013-2019? What are the top 5 counties with the highest number of major wildfire?
     </summary>
    <br> 
  
    2.1 Go back to the pivot table. Add a filter of "Major Incident: True"
  <img width="603" alt="Screen Shot 2021-08-10 at 9 28 20 AM" src="https://user-images.githubusercontent.com/69986804/128899703-9fda8054-fba7-4c6a-9d14-ea0a5e17a4a3.png" width=50%, height=50%> 

    2.2 Copy and paste the result into a new tab. Add column titles "County" and "# Major Incident". Freeze and bold the titles. 
    2.3 Sort the "# Major Incident" column descendingly.
  
 **Result:** 
  - 383 major wildfire occurred in 2013-2019.
  
  <img width="217" alt="Screen Shot 2021-07-26 at 11 49 35 AM" src="https://user-images.githubusercontent.com/69986804/127042635-aa07e41a-e1ae-480e-b94c-0c2e309a354e.png">
      </details>

<details>
  <summary> Question 3. How has the number of total wildfire changed  over the years? </summary>
  <br>
   
    3.1 Make a new pivot table. Choose "Archive Year" as the row. Add COUNTA "CalFireincident" as Values.
    3.2 Copy and paste the result into a new tab. Add column titles "Year" and "# Wildfire". Freeze and bold the titles. 
    
 **Result:**  
    
  <img width="139" alt="Screen Shot 2021-07-26 at 12 00 09 PM" src="https://user-images.githubusercontent.com/69986804/127043871-06163c5e-17f1-4c94-a1cf-ae441395919b.png">

  </details>
  
<details>
  <summary> Question 4. How has the number of major wildifre changed over the years? </summary>
  <br>
    
    4.1 Go back to the pivot table. Add a filter of "Major Incident: True"
   <img src="https://user-images.githubusercontent.com/69986804/128897271-c795f56a-4f8d-4ca1-a324-6bf33449141d.png" width=50%, height=50%>

    4.2 Copy and paste the result into a new tab. Add column titles "Year" and "# Wildfire". Freeze and bold the titles. 
    
  **Result:**  
  
   <img width="174" alt="Screen Shot 2021-07-26 at 12 01 45 PM" src="https://user-images.githubusercontent.com/69986804/127044073-96142669-4673-4bce-9a3e-0f1d55c5744e.png">

  </details>
  
<details>
  <summary> Question 5. What are the top 3 deadliest wildfire? </summary>
  <br>
  
    5.1 Go to the original tab.  
    5.2 Sort the "Fatalities" column descendingly. 
    5.3 Create a new tab and put the Top 3 most deadliest Fire to it. Include the Name, Fatalities, Year and County. 
    
  **Result:** 
  
  <img width="502" alt="Screen Shot 2021-08-10 at 10 13 25 AM" src="https://user-images.githubusercontent.com/69986804/128904507-fb27dfd7-20df-49a7-9481-2da80632c943.png">
  </details>
  
<details>
  <summary> Question 6. What are the top 3 wildfire with largest burned area? </summary>
  <br>
  
    6.1 Go to the original tab.  
    6.2 Sort the "AcresBurned" column descendingly. 
    6.3 Create a new tab and put the Top 4 most burned Fire to it. Include the Name, AcresBurned, Year and County. 
    
  **Result:**  
  
  <img width="573" alt="Screen Shot 2021-07-27 at 2 55 09 PM" src="https://user-images.githubusercontent.com/69986804/127232686-5a82dd0d-217e-4654-80b4-b5dc8a8943d5.png">
</details>

<details>
  <summary> Question 7. How are trend of areas burned by wildfires in 2013-2019? </summary>
  <br>

    7.1 Create a new pivot table. 
    7.2 Choose "Archive Year" as the row. Add SUM "AcresBurned" as Values.
    
  **Result:** 
   
<img width="237" alt="Screen Shot 2021-08-02 at 3 12 31 PM" src="https://user-images.githubusercontent.com/69986804/127932327-5cf48638-b6f4-4fed-9096-7e982a5a2358.png">

  </details>

<details>
  <summary> Question 8. What were the count of wildfire in each month over 2013-2019? </summary>
  <br>
  
    8.1 Go to the original tab.  Create a new column left to the column "Started" and named it "Started Clean". 
    8.2 In the AF2 cell, type =left(AG2,10). Apply the function to the whole column.
    8.3 Copy and paste the column into a new tab
    8.4 Find and replace - into /. Change the column format into Datetime.
    8.5 Copy and paste the column back to the original tab.
   <img src="https://user-images.githubusercontent.com/69986804/128897627-526f02bd-6e1d-4a9b-a3fa-76178683f25d.png" width=50%, height=50%>
    
    8.6 Create a new pivot table. Choose "Started Clean" as rows and SUM "CalFireincident" as values.
    8.7 Right click one of the cells in the "StartClean" column. Select "Create pivot date group" and "Year-Month". 
   <img src="https://user-images.githubusercontent.com/69986804/128898049-7b8bd6dc-3c1b-4408-a20d-e0bac9723d7d.png" width=50%, height=50%>
    
    8.8 Copy and paste the result into a new tab.
    8.9 Maunally make the year as columns.
   <img src="https://user-images.githubusercontent.com/69986804/128898244-23df6b65-202a-4c8d-841c-d8383da4d2d9.png" width=50%, height=50%>
    
    8.10 Make a chart. 
    
  **Result:** 
   
 <img width="602" alt="Screen Shot 2021-07-27 at 3 26 41 PM" src="https://user-images.githubusercontent.com/69986804/127235575-9ae2e9fd-07da-43a4-ae0c-5d1c24bfb5de.png">
  
  </details>
