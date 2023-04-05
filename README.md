# Excel: Customers' Demographics Analysis
## Aim
- Analyse customers' demographics (genders, income, commute distance, etc.) in relation to their decisions to buy products.

## Skills
1. Data Cleaning
3. Pivot Table
4. Interactive Dashboard

## Step 1: Data Cleaning
First, take a look at the raw dataset.

<img width="899" alt="s5" src="https://user-images.githubusercontent.com/113321447/230013063-a62da8a2-b439-4352-bbe8-11f994d544a1.png"> <br>

It is clear that the raw data has numerous problems:
- Marital status (M/S) and Gender (M/F) has overlapping abbreviation
- Commute Distance is not in suitable format for analysis
- Age is continuous variables, which is not suitable for grouping & analysis

### Create Table
I always start Excel project with creating a table, which allows more uniform calculation and formatting. 

### Change Marital Status and Gender abbreviation.

<img width="203" alt="image" src="https://user-images.githubusercontent.com/113321447/230015404-7d612652-8b1a-4719-9d77-c3b55de21504.png">

### Change "10+..." to ">10..." for logical order

![image](https://user-images.githubusercontent.com/113321447/230015676-ee491a90-ed6a-4fbc-8842-1259d705283d.png)

### Create Age Range using IF function
I breakdown the Age into 3 groups:
- < 36 years old: Young Adult
- 36-60 years old: Middle Age
- Over 60 years old: Elderly <br>

Function: =IFS([@Age]<36,"Young Adult", AND(35<[@Age],[@Age]<61),"Middle Age",[@Age]>60,"Elderly")

<img width="128" alt="image" src="https://user-images.githubusercontent.com/113321447/230015956-3714ec2b-b6d0-4f29-a1df-5232b9c48a95.png">

This is the data after cleaning. 

<img width="925" alt="image" src="https://user-images.githubusercontent.com/113321447/230015030-6003ce30-42f6-419c-bb71-38295043d2f3.png"> <br>

## Step 2: Analyze & Visualize data using Pivot Table
I used PivotTable to get an overview of the trends and relationships.

<img width="399" alt="image" src="https://user-images.githubusercontent.com/113321447/230016958-6a806c27-a855-4f45-b5ed-1a1df0d8397f.png"> <br>

### Step 3: Create Dashboard
I finished the visualization by adding slices 

<img width="569" alt="image" src="https://user-images.githubusercontent.com/113321447/230017190-85675111-c4d3-424e-8b5c-9dc0671c7890.png"> <br>

For details, please refer to the excel file uploaded. 




