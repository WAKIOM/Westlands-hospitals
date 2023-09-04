# Analysis process
## Step 1: The business question(s)
Generally, I am a curious person. It all started when I came across those **_here's how  you can make $1000 per month working online_**. One that caught my eye was helping businesses improve their online presence on Google Maps and optimizing their profiles to appear on searches. Today I am not talking about that though, I am interested in analyzing how hospitals have taken advantage of Google listing for their businesses.
What is listing and claiming your business on Google and why is it important?
_When visitors find your business on Google and see a complete, verified listing, they’ll have more trust that it’s a legitimate business. This encourages more people to call or visit your company and purchase its products. Claiming your business on Google also helps you get found in local search results_ 
If you are curious, check [listing your business on Google](https://www.indeed.com/hire/c/info/claim-business-google#:~:text=If%20you%20claim%20a%20business%20on%20Google%2C%20it%20comes%20up,appears%20on%20your%20business%20listing.) for more.
 Thus our business questions:
1. How many of them have a complete listing?
2. Does the business have a website?
3. Do they have reviews?
4. Do they have a phone number listed?
5. Do they have business operation hours listed?

Part 2
After knowing how the businesses are listed, we want to dive deeper into their profiles.
1. What are the categories of businesses
2. What are the top 5 most reviewed businesses?
3. What are their average ratings
4. When are they opened
5. What time do they open

## Step 2: Data Exploration
The dataset contains 100 rows and 22 columns of raw data. Very dirty
##### Dataset Overview in Excel.
![image](https://github.com/WAKIOM/Westlands-hospitals/blob/main/images/westlands%20hospitals%20dataset.png) 

Out of this data, only 16 columns were relevant to our analysis questions. 
3 columns have no missing values. Why do the other columns have missing values? It is not an entry error, it is because they are unobserved values.
The metadata is as seen below;  

![image](https://github.com/WAKIOM/Westlands-hospitals/blob/main/images/medatata.png)
## Step 3: Modelling and cleaning using Power BI power query editor.
- Removed the unnecessary columns
  
  Explored the columns using the magical power bi `column profile` and `column quality` buttons.
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

  
