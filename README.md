# Splendor Hotel Group
![splendor Hotel](https://github.com/babit25/Speldor_hotel_group/assets/108529070/11aa2c13-fd75-4295-931e-6019572aba77)

[Image credit](https://www.blutour.al/)

# Introduction
This Project is a public project shared on X(Twitter) by [@splendor](https://twitter.com/iam_Uchenna). It is about a fictional Hotel group called Splendor Hotel Group. The following Project brief was Shared with me.

# Project Brief 
Analyzing Booking Data for Splendor Hotel Groups (SHG)
Greetings from Splendor Hotel Groups (SHG). As a recently recruited Business Intelligence Analyst and Data Analyst, you will be essential to our efforts to solve the puzzles buried in our booking data. Renowned hospitality company SHG aims to improve visitor experiences and streamline corporate processes by utilizing data-driven insights. Your task is to thoroughly examine one of our best resorts' past booking data to identify trends, comprehend consumer behavior, and offer useful suggestions for tactical decision-making.

# Project Overview
Your task involves a thorough analysis of a comprehensive dataset, featuring intricate details of bookings, guest demographics, distribution channels, and financial metrics. By applying your analytical prowess, we aim to extract meaningful insights that will not only inform operational improvements but also contribute to the overall success of SHG in delivering unparalleled hospitality.

# Dataset

![Dataset](https://github.com/babit25/Speldor_hotel_group/assets/108529070/60011ef3-6ce0-4e09-bc5f-d31c48afddf4)


Data Dictionary:
The dataset contains 17 columns and 119391 rows. 

The columns are Booking ID,	Hotel, Booking Date, Arrival Date, Lead Time, Nights, Guests, Distribution Channel, Customer Type, Country, Deposit Type, Avg Daily Rate, Status, Status UpdatemCanceled (0/1), Revenue, Revenue Loss


# Objectives of the Analysis

**1.	Booking Patterns**
   
  a. What is the trend in booking patterns over time, and are there specific seasons or months with increased booking activity?
  
  b. How does lead time vary across different booking channels, and is there a correlation between lead time and customer type?


**2.	Customer Behavior Analysis**
   
  a.Which distribution channels contribute the most to bookings, and how does the average daily rate (ADR) differ across these channels?
  
  b. Can we identify any patterns in the distribution of guests based on their country of origin, and how does this impact revenue?

**3.	Cancellation Analysis**
   
a. 	What factors are most strongly correlated with cancellations, and can we predict potential cancellations based on certain variables?

b.	How does the revenue loss from cancellations compare across different customer segments and distribution channels?

**4.	Revenue Optimization**
   
  a. 	What is the overall revenue trend, and are there specific customer segments or countries contributing significantly to revenue?

 b. Can we identify optimal pricing strategies based on the Average Daily Rate (ADR) for different customer types and distribution channels?

**5.	Geographical Analysis**
   
  a. How does the distribution of guests vary across different countries, and are there specific countries that should be targeted for marketing efforts?

  b. 	Is there a correlation between the country of origin and the likelihood of cancellations or extended stays?

**6.	Operational Efficiency**

  a. 	What is the average length of stay for guests, and how does it differ based on booking channels or customer types?
  
  b. 	Are there patterns in check-out dates that can inform staffing and resource allocation strategies?

**7.	Impact of Deposit Types**

  a.	How does the presence or absence of a deposit impact the likelihood of cancellations and revenue generation?

  b. 	Can we identify any patterns in the use of deposit types across different customer segments?

**8.	Analysis of Corporate Bookings**

 a. 	What is the proportion of corporate bookings, and how does their Average Daily Rate (ADR) compare to other customer types?

 b. 	Are there specific trends or patterns related to corporate bookings that can inform business strategies?

**9.	Time-to-Event Analysis**

  a. 	How does the time between booking and arrival date (lead time) affect revenue and the likelihood of cancellations?

  b. 	Are there specific lead time ranges that are associated with higher customer satisfaction or revenue?

**10.	Comparison of Online and Offline Travel Agents**

a.	What is the revenue contribution of online travel agents compared to offline travel agents?

b. 	How do cancellation rates and revenue vary between bookings made through online and offline travel agents?

# Tools and Technologies

The tool used for this project is Power Bi 

# Data Cleaning and Transformation

The data was relatively clean. After Loading into Power BI, I checked to make sure the columns were formatted properly.

I created measures to calculate Averages and sums. The measures are; Average Duration (Average nights spent), Average Daily rate (Average of the Avg. Daily rate), cancellation rate, Number of Bookings (Count of Bookings), Number of Guest (sum of guests), Total Revenue (Sum of Revenue), and Total Revenue Loss (Sum of Revenue Loss).

I created a column to calculate the checkout date by adding the number of nights to the arrival dates.

I also grouped the lead time into 4 groups as follows:

_Short Time 	    	- 	0 - 60 Days_

_Medium Time	    - 	61 – 150 Days_

_Long Time	    	- 	151 – 365 Days_

_Extended Time  	- 	365+ Days_

# Preliminary Analysis
![Preliminary Analysis](https://github.com/babit25/Speldor_hotel_group/assets/108529070/f2645c73-0456-467f-99c5-172803397334)



The Group has 2 Hotels which are City hotels and resorts. The total Bookings made was 119,390 and the Total Revenue raised was $ 29,600,597. A loss of $ 13,122,900 was incurred leaving a Net Revenue of $ 16,477,697.
The total number of guests was 234,988 from 175 countries.  The average Days spent and Average Daily rate were 3 days and $ 101.83 respectively.

# Analysis

**1.	Booking Patterns**

    a.	What is the trend in booking patterns over time, and are there specific seasons or months with increased booking activity?

![Number of Bookings by Month and Year](https://github.com/babit25/Speldor_hotel_group/assets/108529070/d33c4e26-da7c-49c1-a9e3-16e68000da73)


![Number of Bookings by Quarter](https://github.com/babit25/Speldor_hotel_group/assets/108529070/f37cd133-aa1b-4fea-9001-a455f747fee7)



2016 had the highest number of Bookings with 58,543 Bookings.  The first quarter had the highest bookings (34%) with January having 14% of the total Bookings.



    b.	How does lead time vary across different booking channels, and is there a correlation between lead time and customer type?

![Average lead time by Distribution channel](https://github.com/babit25/Speldor_hotel_group/assets/108529070/e34cb617-2e72-4fd4-a350-06252acaf225)



![Average Lead time by customer type](https://github.com/babit25/Speldor_hotel_group/assets/108529070/51a8b6a0-fc22-4afc-ac53-8b25c7be2a4a)


 Bookings made via Offline Travel Agents had the longest Average Lead time. Contract Customers had the Longest Average Lead time.

 
 

![Booking Patterns](https://github.com/babit25/Speldor_hotel_group/assets/108529070/cf057a56-479b-422f-ad47-7b68579df2c6)





**2.	Customer Behavior Analysis**

    a.	Which distribution channels contribute the most to bookings, and how does the average daily rate (ADR) differ across these channels?
    

 ![Number of Bookings by Distribution Channel](https://github.com/babit25/Speldor_hotel_group/assets/108529070/161cef19-d25c-40fe-b2a7-3b3e4ea1f7f8)

    
    
![Average Daily rate of Distribution Channels](https://github.com/babit25/Speldor_hotel_group/assets/108529070/5e6a81db-ba98-460f-b3d7-c99842cbf72f)


 Bookings made through Online Travel Agency had 62% of the Bookings. Offline Travel Agency and direct channels follow with 20% and 12% respectively.

Bookings made via Online Travel Agency had the highest Average Daily Rate of all Distribution Channels with $ 108.57 which is greater than the Average Daily rate of $ 101.83.


    b.	Can we identify any patterns in the distribution of guests based on their country of origin, and how does this impact revenue?
    

![Number of guests and Revenue of Countries](https://github.com/babit25/Speldor_hotel_group/assets/108529070/77504518-5d4d-4a82-a42f-3674d11e5341)

    
European Countries accounted for 8 of the Top 10 countries with the highest number of guests. Countries with a higher number of guests bring in more revenues. Portugal had the highest number of guests and revenue with 90036 guests and $ 9,037,388 respectively.



![Customer behaviour](https://github.com/babit25/Speldor_hotel_group/assets/108529070/031de39b-2f3e-4039-b4c2-ccbe65adfd22)




**3.	Cancellation Analysis**

    a.	What factors are most strongly correlated with cancellations, and can we predict potential cancellations based on certain variables?
    

![canceled booking by deposit type](https://github.com/babit25/Speldor_hotel_group/assets/108529070/707e3b49-4f56-45e0-8f61-ae11a4b25ccc)


![canceled booking by distribution channel](https://github.com/babit25/Speldor_hotel_group/assets/108529070/3492b3ce-8ccc-4421-8d4e-5c0ddf2662e2)


The No- Deposit payment type has the most canceled Booking, accounting for 66% of canceled Bookings. Bookings made through Online Travel Agency had 73% of the canceled Bookings.




    b.	How does the revenue loss from cancellations compare across different customer segments and distribution channels?
    

  ![revenue and revenue loss by customer type](https://github.com/babit25/Speldor_hotel_group/assets/108529070/78bcc3c5-f9b2-4493-8764-8cc25fc90489)

  
![revenue and revenue loss by distribution channel](https://github.com/babit25/Speldor_hotel_group/assets/108529070/e4c79759-ea0a-4caa-8263-0768976fb638)


The highest Revenue and revenue loss was by Transient Customer, losing about $12M of the $23M generated revenue.
For Distribution channels, the highest Revenue and revenue loss was by customers who made Bookings via Online Travel Agency.



![Cancellation](https://github.com/babit25/Speldor_hotel_group/assets/108529070/98c19fee-8587-42f4-a2e5-3038188b3676)




**4.	Revenue Optimization**

    a.	What is the overall revenue trend, and are there specific customer segments or countries contributing significantly to revenue?
    

![Total Revenue by countries](https://github.com/babit25/Speldor_hotel_group/assets/108529070/6ce3d525-cb23-4790-aa15-eebe82bd2877)


![Total Revenue by Customer Type](https://github.com/babit25/Speldor_hotel_group/assets/108529070/7f654eb2-71ce-4ab2-a4d1-4284293d4622)


![Total revenue by month and year](https://github.com/babit25/Speldor_hotel_group/assets/108529070/2620a372-3ee8-4acc-9c08-ebdd49a0b55b)

    
 Portugal with 37% of the total revenue generated the most revenue in terms of location of guests with the United Kingdom and France also generating 17% and 13 % of the revenue. Transient customers generated 77% of the Total Revenue.

The highest Revenue was generated in 2016 with $13.92 M. The first quarter of the years 2016 and 2017 contributes more to the revenue.



    b.	Can we identify optimal pricing strategies based on the Average Daily Rate (ADR) for different customer types and distribution channels?
    

 ![AVG customer type ](https://github.com/babit25/Speldor_hotel_group/assets/108529070/b4ba31af-4623-4d58-8932-50c5154a0fc7)


Both online Travel agents and direct channels of distribution have average daily rates of $108.57 and $106.65 respectively. Offline Travel agent has an average daily rate of $87.15.



![Revenue Optimization](https://github.com/babit25/Speldor_hotel_group/assets/108529070/6ee19da6-ff45-495b-ae1e-0df591194a03)




**5.	Geographical Analysis**

    a.	How does the distribution of guests vary across different countries, and are there specific countries that should be targeted for marketing efforts?

![country map](https://github.com/babit25/Speldor_hotel_group/assets/108529070/083ae535-9fc6-4f53-9cea-11f09ba0f544)

    
European countries such as Portugal, the United Kingdom, France, Spain, and Germany make the Top 5 Countries with guests.


    b.	Is there a correlation between the country of origin and the likelihood of cancellations or extended stays?

    
![Number of guest against cancellation rate](https://github.com/babit25/Speldor_hotel_group/assets/108529070/3b48f1c6-c160-46b4-9c54-c58bc58f407d)



With a correlation coefficient of 0.04, there is no correlation between country and cancelation rate.



![Geographical](https://github.com/babit25/Speldor_hotel_group/assets/108529070/037e9410-89f8-4458-8ad3-00c1fa959a7d)



**6.	Operational Efficiency**

    a.	What is the average length of stay for guests, and how does it differ based on booking channels or customer types?

    
![Duration](https://github.com/babit25/Speldor_hotel_group/assets/108529070/e1904a03-41cc-4db6-a6fe-8c7eb5cd35d3)

    
 The average length of stay of customers is 3 Nights with the maximum and most popular nights 69 and 2 respectively. 
 
 
 ![average Duration by Customer type](https://github.com/babit25/Speldor_hotel_group/assets/108529070/9d629311-c545-4367-8c3f-b6c853487b63)
 
 
 Contract Customers tend to stay the longest with an average of 5. The other groups have an average of 3 Nights.
 
 
 ![Average Duration by distribution channel](https://github.com/babit25/Speldor_hotel_group/assets/108529070/7004df2c-2f0d-4ecb-96d5-831e8971d8b4)

 
 With 4 Nights, Customers who make bookings via offline travel agents stay longer Nights than other customers with 3.


    b.	Are there patterns in check-out dates that can inform staffing and resource allocation strategies?
    

![checkout day](https://github.com/babit25/Speldor_hotel_group/assets/108529070/b95cfc29-0775-4fa4-b28c-927f76c02b2f)

    
Sundays are the most popular check-out day, with Thursday and Friday coming second and third respectively.



![Operation Efficiency](https://github.com/babit25/Speldor_hotel_group/assets/108529070/dff15bc7-f83a-44fe-b266-97f650f2de8e)




**7.	Impact of Deposit Types**

    a.	How does the presence or absence of a deposit impact the likelihood of cancellations and revenue generation?
    
    
   
    
 ![cancellation rate by deposit type](https://github.com/babit25/Speldor_hotel_group/assets/108529070/74c876fb-2f53-4f7e-a59c-d3c692f500aa)

 
 Non-refundable deposit type had the highest Cancelation at 0.99. This shows that the absence of a deposit makes it likely to cancel. 
 
 
 ![revenue and revenue loss by deposit type](https://github.com/babit25/Speldor_hotel_group/assets/108529070/ccf1fd3a-ec33-4aa6-bc91-22280ad56f05)

 
 The Net Revenue for the No-Deposit type is $12.85 M with Non-Refundable at $ 3.62 M and Refundable at $ 8999.04
 

    b.	Can we identify any patterns in the use of deposit types across different customer segments?

    
![Customer by deposit type](https://github.com/babit25/Speldor_hotel_group/assets/108529070/415f0c1d-7bd1-4ec4-a828-ae687ff215e5)


The No-Deposit type was the most popular Deposit type among all customer types. 85% of Transient customer types used No-Deposit, with 95%, 87%, and, 98% for party, contract, and group respectively.




![Deposit Types](https://github.com/babit25/Speldor_hotel_group/assets/108529070/0188de0d-d85b-4d9a-94ef-b1534ab80b51)




**8.	Analysis of Corporate Bookings**

    a.	What is the proportion of corporate bookings, and how does their Average Daily Rate (ADR) compare to other customer types?
    

    


![corporate bookings](https://github.com/babit25/Speldor_hotel_group/assets/108529070/9bce36e2-4907-4b73-874e-11aab8d38411)


There were 6677 Corporate Bookings which amount to 5.59 % of the Total Bookings.


![Average Daily rate of Distribution Channels](https://github.com/babit25/Speldor_hotel_group/assets/108529070/b8aab44f-1939-43ec-a84a-e5dd58f111b4)


Average Daily rate (ADR) of Corporate Booking is the 4th highest ADR, 32% lower than the ADR of all customers


    b.	Are there specific trends or patterns related to corporate bookings that can inform business strategies?
    


    

![corporate booking by month](https://github.com/babit25/Speldor_hotel_group/assets/108529070/09414482-0ddc-4ff2-b20d-4f0c473d79a7)


Most Corporate Bookings are made in January, October, and March respectively. January with 773 bookings is 12% of all corporate bookings.



![Corporate Booking](https://github.com/babit25/Speldor_hotel_group/assets/108529070/80d0005e-5d32-41df-a824-7dce67b80c98)




**9.	Time-to-Event Analysis**

    a.	How does the time between booking and arrival date (lead time) affect revenue and the likelihood of cancellations?
    

 


 ![revenue by lead time](https://github.com/babit25/Speldor_hotel_group/assets/108529070/5a3bffef-8e0c-4ea7-9664-ced3f3de7563)

    
![cancellation rate by lead time](https://github.com/babit25/Speldor_hotel_group/assets/108529070/db97ea24-d1f7-404b-ac38-666c69975e81)



Short Time had the highest Total Revenue while Extended Time had the lowest Total RevenueS hort Time accounted for 40.08% of Total Revenue. The shorter the Lead time the lower the cancellation rate.



**10.	Comparison of Online and Offline Travel Agents**

    a.	What is the revenue contribution of online travel agents compared to offline travel agents?
    

![revenue by distribution channel](https://github.com/babit25/Speldor_hotel_group/assets/108529070/b578618b-15ef-4e24-bacf-90690575f9cc)

    
Online travel agents' booking channels bought $2.04M while Offline Booking agents $1.37M in revenue.


b.	How do cancellation rates and revenue vary between bookings made through online and offline travel agents?

![cancellation rate by distribution channel](https://github.com/babit25/Speldor_hotel_group/assets/108529070/b31277a3-6cbf-405e-ad1b-a7a63c9bd98b)


Online travel agents' booking channels brought in more Revenue and accounted for 60% of revenue bought in by both distribution channels.
cancelation rate was higher with online travel agents.



![Time to Event](https://github.com/babit25/Speldor_hotel_group/assets/108529070/21095a78-bd05-4a03-93e1-005c01738f0d)



# Dashboard
I created a dashboard to showcase important findings with filters.



![Dashboard](https://github.com/babit25/Speldor_hotel_group/assets/108529070/e0d09c08-4665-46b5-83e5-a34e96000dd7)


# Insights

1. Guests with European origins are the major customers of the Hotel group.
   
2. The first and last quarters are the busiest periods of the hotel
   
3. Online travel agents are the most utilized distribution channel for Bookings.
   
4. The busiest day in terms of guest checkout is Sunday.
   
5. Cancellations were mostly influenced by the No-deposit payment method which led to loss of revenue.

   
# Recommendations

1. marketing efforts should be concentrated mostly in European countries. promotions, such as discounts should also be offered to guests from other continents
   
2. Lead time beyond 12 months should be discouraged.
   
3. A high number of Staff should be available on Sundays and Mondays as it is the most likely day for check-outs
   
4. No-payment method should be revised and replaced with non-refundable deposits. This will reduce cancellations and revenue loss associated with it

# Conclusion
The Splendor Hotel Group is currently doing okay. I believe my recommendations, if implemented would increase the revenue and popularity of the group.


Thank you



![BABIT](https://github.com/babit25/Speldor_hotel_group/assets/108529070/ace8776a-bca8-465e-830b-ceb34fa894c5)















