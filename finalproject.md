# J124 Data Journalism Final Project: California Wildfires 2013-2019 
By Winnie Lau, Journalism student at the University of California Berkeley 

Data: 2013-2019 California wildfires dataset from California Department of Forestry and Fire Protection (Cal Fire)

## Part 1. Story Summary and Sourcing</summary>

### Data Analysis Summary (More detailed analysis process in Part 3)

**Number of wildfire**

- The wildfires were concentrated in Riverside and San Diego counties in Southern California and Butte county in Northern California. 
- The number of wildfires has increased 2.7 times from 162 in 2013 to 438 in 2017 and then dropped to 266 in 2019. 

**Severeness of Wildfires**

- The size of wildfire fluctuated between 450 thousands to 600 thousands acres in 2013-2016 and significantly increased to 1.7 million in 2017 and even 3.4 million acres in 2018. It dropped to 280 thousand acres in 2019. 
- The top 3 counties with the largest acres burned are Lake, Mendocino, and Trinity near the Northern California Coast. 
- The top 3 deadliest wildifires occurred in Northern California in 2017 and 2018 -- Camp Fire (2018) in Butte County, Tubbs Fire (2017) in Napa and Sonoma counties, and Redwood Valley Fire (2017) in Mendocino county.
  - Camp Fire remains the deadliest wildfire in California's history. 

**Timing**

- The data also shows that there is a trend of wildfires starting later than previous years. 

### Additional Sources

- Statistics of wildfires on CalFire website (https://www.fire.ca.gov/stats-events/)
  -  it tells us the most updated statistics, including the fires in 2020 and 2021. 
  
- The report on "Top 20 Largest California Wildfires" by CalFire (https://www.fire.ca.gov/media/4jandlhh/top20_acres.pdf), 
  -  it tells us the trend of more severe wildfire in California. 
  -  The report shows that five out of the top 6 largest California Wildfires occurred in 2020 and 2021. 
  -  The acres burned by the 2020 August Complex and active 2021 Dixie Fire have surpassed the Mendocino Complex in 2018 which was the largest wildfire in 2013-2019. 

### Story Idea

Based on the findings, we see a trend of increaing number and severeness of wildfires. This data story will be about the trend of California wildfire and the atmospheric and geographical factors affecting the scale and severeness of the wildfires. In particular, the story will focus on the relationship between climate change and the severeness of wildfire. 

### Human Sources

- CalFire Northern Region Chief,	Mike Bradley, (530) 224-2460, and CalFire Southern Region Chief,	Dave Fulcher,	 (559) 243-4127 for their comments on the wildfire trend. 
- Experts in wildfires, for example, 
  - UCLA Climate scientist, Daniel Swain, PhD, (dlswain@ucla.edu). 
    - He studies how the atmospheric phenomena increases the risk of severe wildfires. His insight would add the relationship between climate change and wildfire to the story. 
  - UC Davis Department of Public Health Sciences Professor Irva Hertz-Picciotto (ihp@ucdavis.edu). 
    - She studies the potential health impacts of wildfire, smoke and ash. She would add the impact of wildfires to the story. 

## Part 2. Data Visualization

<img src="https://user-images.githubusercontent.com/69986804/129123310-dac63066-73b5-4020-b49a-d8b41b30c75b.png" width=50% height=50%><img src="https://user-images.githubusercontent.com/69986804/129134117-4c2f223f-62fa-4357-82a4-c053f1ceece1.png" width=50% height=50%>

Link to the map "Number of Wildfires in California in 2013-2019": https://www.datawrapper.de/_/EKQT7/

Link to the map "Acres Burned by Wildfires in California in 2013-2019": https://www.datawrapper.de/_/DbONi/

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
    - There are entries of the same fire but in different counties, so we should keep them. 

**Step 5: Think of questions for the dataset, analyze the data and find the answers**

<details>
  <summary> Question 1. How many wildfire in total in 2013-2019? What are the top 5 counties with the highest number of wildfire? 
    
  - 1636 wildfire occurred in 2013-2019.

 <img width="220" alt="Screen Shot 2021-07-26 at 11 35 26 AM" src="https://user-images.githubusercontent.com/69986804/127040763-3c4f3f79-d91e-4863-bb25-bfe15a958cd5.png">
 <img src="https://user-images.githubusercontent.com/69986804/129237813-f7e006f9-f7cf-4915-a544-a3af3dd4de64.png" width=50%, height=50%>

  </summary>
    <br>
  Steps
  
    1.1 Create a pivot table, choose "Counties" as the rows, and add COUNTA "CalFireincident" as Values.
  <img src="https://user-images.githubusercontent.com/69986804/128896978-96dc59e9-9083-4c7a-9951-2656dd5b029c.png" width=50%, height=50%>

    1.2 Copy and paste the result into a new tab. Add column titles "County" and "# WildFire". Freeze and bold the titles. 
    1.3 Sort the "# WildFire" column descendingly.


</details>
    
<details>
  <summary>
    Question 2. How many major wildfire in 2013-2019? What are the top 5 counties with the highest number of major wildfire?
    
  - 383 major wildfire occurred in 2013-2019.
  
  <img width="217" alt="Screen Shot 2021-07-26 at 11 49 35 AM" src="https://user-images.githubusercontent.com/69986804/127042635-aa07e41a-e1ae-480e-b94c-0c2e309a354e.png">
  <img src="https://user-images.githubusercontent.com/69986804/129237839-6784cfd7-7b5a-4f4a-9149-507e917a4f20.png" width=50%, height=50%>

   </summary>
   <br> 
  
  Steps
    2.1 Go back to the pivot table. Add a filter of "Major Incident: True"
  <img width="603" alt="Screen Shot 2021-08-10 at 9 28 20 AM" src="https://user-images.githubusercontent.com/69986804/128899703-9fda8054-fba7-4c6a-9d14-ea0a5e17a4a3.png" width=50%, height=50%> 

    2.2 Copy and paste the result into a new tab. Add column titles "County" and "# Major Incident". Freeze and bold the titles. 
    2.3 Sort the "# Major Incident" column descendingly.

 </details>

<details>
  <summary> Question 3. How has the number of total wildfire changed  over the years? <br>
    
 <img width="139" alt="Screen Shot 2021-07-26 at 12 00 09 PM" src="https://user-images.githubusercontent.com/69986804/127043871-06163c5e-17f1-4c94-a1cf-ae441395919b.png">
 <img src="https://user-images.githubusercontent.com/69986804/129233680-7affec1a-dd3f-41ee-956e-ea503ea18a04.png" width=50%, height=50%>
  
  </summary>
  <br>
   
  Steps
  
    3.1 Make a new pivot table. Choose "Archive Year" as the row. Add COUNTA "CalFireincident" as Values.
    3.2 Copy and paste the result into a new tab. Add column titles "Year" and "# Wildfire". Freeze and bold the titles. 
   
  </details>
  
<details>
  <summary> Question 4. How has the number of major wildifre changed over the years?<br>
    
 <img width="174" alt="Screen Shot 2021-07-26 at 12 01 45 PM" src="https://user-images.githubusercontent.com/69986804/127044073-96142669-4673-4bce-9a3e-0f1d55c5744e.png">
 <img src="https://user-images.githubusercontent.com/69986804/129233700-f99027d5-b04b-4f09-a343-8336d999a465.png" width=50%, height=50%>

  
  </summary>
  <br>
  
  Steps
    
    4.1 Go back to the pivot table. Add a filter of "Major Incident: True"
   <img src="https://user-images.githubusercontent.com/69986804/128897271-c795f56a-4f8d-4ca1-a324-6bf33449141d.png" width=50%, height=50%>

    4.2 Copy and paste the result into a new tab. Add column titles "Year" and "# Wildfire". Freeze and bold the titles. 
   
  </details>
  
<details>
  <summary> Question 5. What are the top 3 deadliest wildfire? <br>
    
 <img width="502" alt="Screen Shot 2021-08-10 at 10 13 25 AM" src="https://user-images.githubusercontent.com/69986804/128904507-fb27dfd7-20df-49a7-9481-2da80632c943.png">
  
  </summary>
  <br>
  
  Steps
  
    5.1 Go to the original tab.  
    5.2 Sort the "Fatalities" column descendingly. 
    5.3 Create a new tab and put the Top 3 most deadliest Fire to it. Include the Name, Fatalities, Year and County. 
   
  </details>
  
<details>
  <summary> Question 6. What are the top 3 wildfire with largest burned area? 
    <img width="573" alt="Screen Shot 2021-07-27 at 2 55 09 PM" src="https://user-images.githubusercontent.com/69986804/127232686-5a82dd0d-217e-4654-80b4-b5dc8a8943d5.png">
  
  </summary>
  <br>
  
  Steps
  
    6.1 Go to the original tab.  
    6.2 Sort the "AcresBurned" column descendingly. 
    6.3 Create a new tab and put the Top 4 most burned Fire to it. Include the Name, AcresBurned, Year and County. 

</details>

<details>
  <summary> Question 7. How is trend of areas burned by wildfires in 2013-2019? <br>
    <img width="237" alt="Screen Shot 2021-08-02 at 3 12 31 PM" src="https://user-images.githubusercontent.com/69986804/127932327-5cf48638-b6f4-4fed-9096-7e982a5a2358.png">
   <img src="https://user-images.githubusercontent.com/69986804/129234137-483a5613-be1c-432d-bae0-9fcf11e09d09.png" width=50%, height=50%>


  </summary>
  <br>

  Steps
  
    7.1 Create a new pivot table. 
    7.2 Choose "Archive Year" as the row. Add SUM "AcresBurned" as Values.
    
  </details>

<details>
  <summary> Question 8. What were the numbers of wildfire in each month in 2013-2019?
   <img width="602" alt="Screen Shot 2021-07-27 at 3 26 41 PM" src="https://user-images.githubusercontent.com/69986804/127235575-9ae2e9fd-07da-43a4-ae0c-5d1c24bfb5de.png">
  
  </summary>
  <br>
  
  Steps
  
    8.1 Go to the original tab.  Create a new column left to the column "Started" and named it "Started Clean". 
    8.2 In the AG2 cell, type =left(AH2,10). Apply the function to the whole column.
<img width="289" alt="Screen Shot 2021-08-11 at 10 10 25 PM" src="https://user-images.githubusercontent.com/69986804/129141443-05adde90-d8ae-4dec-8f2c-235e2c18eec6.png">

    8.3 Created a new sheet and then copy and paste the column into it. Use "Paste with values only". 
  <img width="562" alt="Screen Shot 2021-08-11 at 10 10 38 PM" src="https://user-images.githubusercontent.com/69986804/129141500-1d310619-2bed-4f10-bd75-6cc701540f87.png">

    8.4 Find and replace - into /.
  <img width="492" alt="Screen Shot 2021-08-11 at 10 12 50 PM" src="https://user-images.githubusercontent.com/69986804/129141641-d9b5f13c-271d-4eba-aeb0-a1e7cd444d8d.png">

    8.5 Change the column format into Date.
  
  <img width="551" alt="Screen Shot 2021-08-11 at 10 15 08 PM" src="https://user-images.githubusercontent.com/69986804/129141815-7cca6e58-ef3b-4657-9e98-2eba7ae9d690.png">

    8.6 Copy and paste the column back to the original tab.
    8.7 Create a new pivot table. Choose "Started Clean" as rows and SUM "CalFireincident" as values.
    8.8 Right click one of the cells in the "StartClean" column. Select "Create pivot date group" and "Year". 
  
  <img width="830" alt="Screen Shot 2021-08-11 at 10 18 40 PM" src="https://user-images.githubusercontent.com/69986804/129142153-93dfe71a-4606-48b9-9232-e19c580808b6.png">
  
    8.9 Add one more row of "Started Clean" and select ""Create pivot date group" and "Year-Month". 
  
  <img width="832" alt="Screen Shot 2021-08-11 at 10 19 01 PM" src="https://user-images.githubusercontent.com/69986804/129142276-21902047-1c17-4e25-bde1-b167755565a4.png">
    
    8.10 Copy and paste the result into a new tab.
    8.11 Maunally make the year as columns.
    8.12 Make a chart on Google Sheet. 
  
  <img width="734" alt="Screen Shot 2021-08-11 at 10 23 26 PM" src="https://user-images.githubusercontent.com/69986804/129142520-e007499c-fae4-484b-9fdd-07eb520f76c5.png">
  
  </details>
