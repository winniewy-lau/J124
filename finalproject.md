# J124
Intro to Data Journalism Markdown Final Project Process

Step 1: download the cvs file dataset from https://www.kaggle.com/ananthu017/california-wildfire-incidents-20132020.

Step 2: import the cvs file into Google Drive and open it as Google Form.

Step 3: Clean the dataset
  - freeze and bold the first row
  - look for error or anomalies

Step 4: Think of questions for the dataset
  1. How many total wildfire? What are the top 5 counties with the highest number of wildfire?
  2. How many total major wildfire? What are the top 5 counties with the highest number of major wildfire?
  3. How has the number of total wildfire changed  over the years?
  4. How has the number of major wildifre changed over the years?
  5. What are the top 3 wildfire with the most injuries?
  6. What are the top 4 wildfire with burnt the largest area?
  7. How is the started months of wildfire changed in 2013-2019?

Step 5: Analyze the data and find the answers

First, bold and freeze the column names. 

Question 1

    1.1 Create a pivot table, choose "Counties" as the rows, and add COUNTA "CalFireincident" as Values.
    1.2 Copy and paste the result into a new tab. Add column titles "County" and "# WildFire". Freeze and bold the titles. 
    1.3 Sort the "# WildFire" column descendingly.
  Result: 
  - 1636 wildfire occurred in 2013-2019.

 <img width="220" alt="Screen Shot 2021-07-26 at 11 35 26 AM" src="https://user-images.githubusercontent.com/69986804/127040763-3c4f3f79-d91e-4863-bb25-bfe15a958cd5.png">
 
 Question 2
 
    2.1 Go back to the pivot table. Add a filter of "Major Incident: True"
    2.2 Copy and paste the result into a new tab. Add column titles "County" and "# Major Incident". Freeze and bold the titles. 
    2.3 Sort the "# Major Incident" column descendingly.
  Result:
  - 383 major wildfire occurred in 2013-2019.
  
  <img width="217" alt="Screen Shot 2021-07-26 at 11 49 35 AM" src="https://user-images.githubusercontent.com/69986804/127042635-aa07e41a-e1ae-480e-b94c-0c2e309a354e.png">
  
 Question 3
 
    3.1 Make a new pivot table. Choose "Archive Year" as the row. Add COUNTA "CalFireincident" as Values.
    3.2 Copy and paste the result into a new tab. Add column titles "Year" and "# Wildfire". Freeze and bold the titles. 
    
 Result: 
    
  <img width="139" alt="Screen Shot 2021-07-26 at 12 00 09 PM" src="https://user-images.githubusercontent.com/69986804/127043871-06163c5e-17f1-4c94-a1cf-ae441395919b.png">

  Question 4
  
    4.1 Go back to the pivot table. Add a filter of "Major Incident: True"
    4.2 Copy and paste the result into a new tab. Add column titles "Year" and "# Wildfire". Freeze and bold the titles. 
    
  Result: 
  
   <img width="174" alt="Screen Shot 2021-07-26 at 12 01 45 PM" src="https://user-images.githubusercontent.com/69986804/127044073-96142669-4673-4bce-9a3e-0f1d55c5744e.png">

  Question 5

    5.1 Go to the original tab.  
    5.2 Sort the "Injuries" column descendingly. 
    5.3 Create a new tab and put the Top 3 most injuried Fire to it. Include the Name, Injuries, Year and County. 
    
  Result:
  
    <img width="439" alt="Screen Shot 2021-07-26 at 12 08 59 PM" src="https://user-images.githubusercontent.com/69986804/127045061-ff252d31-f511-47c7-8865-8d287947cae2.png">
    
  Question 6

    6.1 Go to the original tab.  
    6.2 Sort the "AcresBurned" column descendingly. 
    6.3 Create a new tab and put the Top 4 most burned Fire to it. Include the Name, AcresBurned, Year and County. 
    
  Result: 
  
  <img width="573" alt="Screen Shot 2021-07-27 at 2 55 09 PM" src="https://user-images.githubusercontent.com/69986804/127232686-5a82dd0d-217e-4654-80b4-b5dc8a8943d5.png">


  Question 7

    7.1 Go to the original tab.  Create a new column left to the column "Started" and named it "Started Clean". 
    7.2 In the AF2 cell, type =left(AG2,10). Apply the function to the whole column.
    7.3 Copy and paste the column into a new tab.
    7.4 Find and replace - into /. Change the column format into Datetime.
    7.5 Copy and paste the column back to the original tab.
    7.6 Create a new pivot table. Choose "Started Clean" as rows and SUM "CalFireincident" as values.
    7.7 Right click one of the cells in the "StartClean" column. Select "Create pivot date group" and "Year-Month". 
    7.8 Copy and paste the result into a new tab.
    7.9 Maunally make the year as columns.
    7.10 Make a chart. 
    
   Result:
   
   <img width="601" alt="Screen Shot 2021-07-27 at 2 25 51 PM" src="https://user-images.githubusercontent.com/69986804/127229567-9353d882-d5de-4ee3-a8dd-182e1992d985.png">

    

    
