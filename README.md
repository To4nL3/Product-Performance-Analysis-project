# Product-Performance-Analysis-project
# THE DATA:

The data is an Excel file downloaded from Kaggle.com, a data center with many datasets worldwide. This dataset uses the years from December 1, 2009, to December 9, 2011.

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/b6217781-b8a8-4bfa-9068-f44919c152f0).

It contains 2 Excel sheets of 2 different years, “2009-2010 and “2010-2011” with 9 columns
and 525462 rows in year 2009-2010 sheet and 9 columns and 541911 rows in year 2010-2011 sheet. Below is an image of the columns and their descriptions.

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/fc11ed28-e098-4924-b804-3fbb1f7e24a1)

## OBJECTIVES

The purpose of this analysis is to analyze an online retail store dataset. Here are several questions that will be answered in this analysis:
1.	What is the total amount of revenue generated?
2.	What products do consumers buy most?
3.	Which product is the most expensive?
4.	Which product has the highest total sales?
5.	Which countries do most customers come from?
6.	How many products were canceled?

## TOOLS

I use Python 3.12 as my primary data tool for the processes of data cleaning, analysis, and visualization in Excel.

DATA PREPARATION:
In the data preparation section, I will prepare the data so that the data is clean and can be analyzed properly in the next section. The following is the Python code that I used to do the data preparation.

*Import openpyxl as pd
This library uploads Excel in Python 3.12

After adding the libraries, the next step is to call the dataset downloaded from Kaggle.

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/e9548c0b-50d2-4b81-bb46-b495e1088774)

Here are some of the data from my dataset:

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/d0653dff-1077-4ed0-bff0-5bd0f9a951ad)


## DATA CLEANING

To work with the data I did the Data cleaning first as this is an important part in data analysis. In this way, we will be able to understand if the data seen is ready to be analyzed or not. If not, then cleaning can be done. Cleaning can be done by removing outliers, empty values, and duplicate data.

Handle missing data: First, I would look at the amount of missing data in each column.

> dataset.isnull().sum()

The above data code gives the columns whose data is missing, the Description column and Customer ID. And to delete rows with missing data, I used the following code:

> delete rows with missing data dataset1 = dataset.dropna()

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/7e96830a-9e81-4ca1-ac85-c725b0ac3536)

## ANALYSIS
1.	What is the total amount of revenue generated?

To check and analyze data, Python removed the total revenue generated by adding the sum formula in an Excel file for both sheets, Years 2009-2010 and Years 2010-2011.

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/7b4afdeb-069d-4d3a-a939-b120ac556ff1)


2.	Total No. of Customers acquired.

The total no. of unique customer was taken out by customer ID column and adding unique customer ID function in the formula for python to check and analyze data. As per the data total number of unique customers are 5942.

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/4b2cb644-9b2f-4bf7-bde1-4190fc35bb77)


3.	Which is the bestselling product?
 
The best-selling product based on the stock code and quantity of product sold in both years by ignoring negative values and expenses.

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/f699a29f-66ab-41af-93d3-2eb0f5dd0dcb)

For year 2010-2011

| Invoice | StockCode | Desciption |
| ---- | ---- | ---- |
| 556527 | 23343 | JUMBO BAG VINTAGE CHRISTMAS |


For year 2009-2010

| Invoice | StockCode | Desciption |
| ---- | ---- | ---- |
| 500128 | 22467 | GUMBALL COAT RACK |

4.	Country with the highest sales of Product:
   
The UK stands out as the country with the highest number of transactions, totaling 902,5222. This data suggests an opportunity for online retailers to consider increasing their production and marketing efforts within the UK market. However, it's important not to solely focus on the UK; attention should also be
given to countries with lower transaction volumes. Inbound marketing, targeted advertising, and exploring international markets can effectively expand sales abroad.

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/f096e520-5da9-4400-88ac-79b4455a1716)

5.	Products with less quantity sold:

The products with low sales quantities present valuable insights for online stores to initiate strategic actions. It's essential for businesses to delve into the underlying reasons behind the lack of popularity among consumers. Questions arise: Is there a functional deficiency in the product? Is there a genuine demand for it within the target market? Or does its necessity peak during specific times or seasons? Exploring these factors is crucial for informed decision-making and optimizing product offerings.

6.	Products with the highest price:

The PICNIC BASKET WICKER 60 PIECES stands out as the highest-priced product at 649.5 Pound sterling. It's commonly perceived that higher prices correlate with better quality or rarity. However, it's imperative for businesses to ensure that the high price is justified by the product's quality.
Maintaining the quality of the PICNIC BASKET WICKER 60 PIECES is essential to uphold consumer trust and satisfaction. If customers perceive a disconnect between price and quality, it can adversely affect the online store's reputation. Therefore, focusing on quality assurance is crucial to sustain consumer interest and willingness to purchase despite the premium price tag.

![image](https://github.com/To4nL3/Product-Performance-Analysis-project/assets/166645959/f164b379-bead-4dcb-95cd-b41ace95779f)

## RECOMMENDATION
That’s the final part of the online shop analysis this time. Data analysis is a very important thing to do, because with data analysis we can make decisions based on data. Decisions with databases are very powerful compared to decisions taken without data. So the point is to use data in our business, because with data everything can be done well and accurately.
1.	Revenue Analysis:
   
Examine revenue trends between 2009-2010 and 2010-2011 to identify growth or decline patterns. Look for factors contributing to these changes, such as seasonality, product popularity, or economic conditions. Utilize this analysis to refine business strategies and capitalize on revenue opportunities.

2.	Customer Acquisition Strategies:

With 5942 unique customers acquired, focus on building long-term relationships. Implement personalized marketing tactics, loyalty programs, and exceptional customer service to enhance customer satisfaction and retention. Encourage repeat purchases through targeted promotions and incentives.

3.	Best-selling Product Identification:
 
Identify top-selling products like "JUMBO BAG VINTAGE CHRISTMAS" and "GUMBALL COAT RACK" for each respective year. Analyze the unique selling points of these products, such as design, functionality, or seasonal appeal. Leverage this insight to optimize marketing efforts and prioritize product development.

4.	Sales by Country Analysis:

While the UK leads in transaction volume, explore opportunities for international expansion. Evaluate markets with lower transaction numbers (e.g., Netherlands, EIRE, Germany) for potential growth. Tailor marketing strategies and product offerings to resonate with local preferences and consumer behavior.


5.	Low Sales Quantity Product Evaluation:
   
Investigate products with low sales quantities to uncover underlying reasons. Conduct market research to understand customer preferences and demand drivers. Adjust pricing, marketing messaging, or product positioning to stimulate sales and improve product performance.

6.	High-priced Product Strategy:

Ensure that the high-priced product "PICNIC BASKET WICKER 60 PIECES" maintains perceived value and quality. Monitor customer feedback and satisfaction levels to address any concerns promptly. Consider offering unique value propositions or exclusive benefits to justify the premium price and differentiate the product from competitors.

## CLOSING

In conclusion, by carefully analyzing revenue trends, customer acquisition strategies, product performance, and international sales opportunities, businesses can unlock new avenues for growth and success. Remember to continuously monitor and adapt your strategies based on
market dynamics and customer feedback. With a proactive approach to addressing challenges and leveraging opportunities, you can position your business for sustained profitability and
expansion in both domestic and international markets.




