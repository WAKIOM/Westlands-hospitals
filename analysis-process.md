# Hospitals Google Listings Statistics

## Step 1: The business question(s)
Generally, I am a curious person. It all started when I came across those **_here's how  you can make $1000 per month working online_**. One that caught my eye was helping businesses improve their online presence on Google Maps and optimizing their profiles to appear on searches. Today I am not talking about that though, I am interested in analyzing how hospitals have taken advantage of Google listing for their businesses.
What is listing and claiming your business on Google and why is it important?
_When visitors find your business on Google and see a complete, verified listing, they’ll have more trust that it’s a legitimate business. This encourages more people to call or visit your company and purchase its products. Claiming your business on Google also helps you get found in local search results_ 
If you are curious, check [listing your business on Google](https://www.indeed.com/hire/c/info/claim-business-google#:~:text=If%20you%20claim%20a%20business%20on%20Google%2C%20it%20comes%20up,appears%20on%20your%20business%20listing.) for more.
 To our business questions:
 
 #### Part 1
1. How many of them have a complete listing?
2. Does the business have a website?
3. Do they have reviews?
4. Do they have a phone number listed?
5. Do they have business operation hours listed?

#### Part 2

After knowing how the businesses are listed, we want to dive deeper into their profiles.
1. What are the categories of hospitals
2. What are the top 5 most reviewed hospitals?
3. What are the top 5 highest-rated hospitals?
4. When are they opened
5. How many are claimed

## Step 2: Data Exploration
The dataset contained 100 rows and 22 columns of raw data. Very dirty
##### Dataset Overview in Excel.
![image](https://github.com/WAKIOM/Westlands-hospitals/blob/main/images/westlands%20hospitals%20dataset.png) 

Out of this data, only 16 columns were relevant to our analysis questions. 
3 columns had no missing values.
The metadata is as seen below;  

![image](https://github.com/WAKIOM/Westlands-hospitals/blob/main/images/medatata.png)
## Step 3: Modelling and cleaning using Power BI power query editor.
- Removed the unnecessary columns
  
- Explored the columns using the magical power bi `column profile` and `column quality` buttons.
##### Check the columns' distribution.

![column profile](https://github.com/WAKIOM/Westlands-hospitals/blob/main/images/Column%20profile.png)
##### Check for errors and completeness 

![column quality](https://github.com/WAKIOM/Westlands-hospitals/blob/main/images/column%20quality.png)

- Replaced null with zero in the review count column
- Replace missing values with null
- Performed modeling using DAX functions
- Created a new table to hold the calculations I did so that my Original table remains clean.
  The dataset was now ready for cooking.
## Step 4: Data analysis
To answer Part One of our analysis questions, I created this dashboard. It is like a report that comes with recommendations and findings.

![visualization of hospitals google listing profiles](https://github.com/WAKIOM/Westlands-hospitals/blob/main/images/Viz%20Hosps%20Google%20theme.jpg)

To answer part two of the analysis questions

This is an interactive dashboard designed on Power BI. This way anyone can use the slicers to filter the data to answer all the questions.

![visualization](https://github.com/WAKIOM/Westlands-hospitals/blob/main/images/Visualization%20of%20westlandslistings.png)

## Step 5: Findings
+ There are 17 categories of hospitals
  The four most common ones are
  ```
  Hospital
  Medical Center
  Medical Clinic
  Children's hospital
  ```
+ The top 5 most reviewed hospitals are;
 ```
 The Nairobi West Hospital
 The Nairobi Hospital's Doctor's Plaza
 MP Shah Hospital
 Avenue healthcare Nairobi
 DR Agarwals Eye Hospital Nairobi
```
+ The highest-rated hospitals
  Merit is that they have at least 50 reviews.
   
```
Westlands Laser Eye Hospital
DR Agarwals Eye Hospital Nairobi
The Nairobi West Hospital
Guru Nanak Ramgarhia Sikh Hospital
Meditest Hospital
```
+ Only 19 out of 100 hospitals are open 24 hours
+ 56 hospitals open during weekends
+ Only 83  hospitals are claimed.

