# Data-Science-Challenge

## Question 1:
 
 On Shopify, we have exactly 100 sneaker shops, and each of these shops sells only one model of shoe. We want to do some analysis of the average order value (AOV). When we look at orders data over a 30 day window, we naively calculate an AOV of $3145.13. Given that we know these shops are selling sneakers, a relatively affordable item, something seems wrong with our analysis. 

1. Think about what could be going wrong with our calculation. Think about a better way to evaluate this data.
2. What metric would you report for this dataset?
3. What is its value?

## Answers: 

1. The incorrect AOV calculation of $3145.13 was most likely arrived at by mistakenly calculating the total_items with the count() function instead of sum().count() will only provide the total count of the number of rows . Sum() will add together all of the values in the total_items column. So will get Sum(order_amount)/5000=3145.13, which is heavy number. If we use function Sum(), we will get  Sum(order_amount)/43936=357.92.

2. To determine the correct Average Order Value (AOV), the reporting metrics are the respective sums of both 'order_amount' and 'total_items':<br/>

   for i in range(1,maxlum+1):
   if sheet.cell(1,i).value=='order_amount':#get column of order_amount
        oa=i
   elif sheet.cell(1,i).value=='total_items':#get column of total_items
        ti=i
   for i in range(2,maxrow+1):
        oasum=oasum+sheet.cell(i,oa).value #get the sum of order_amount
   print(oasum)
   for i in range(2,maxrow+1):
        tisum=tisum+sheet.cell(i,ti).value #get the sum of total_items


3. The Average Order Value (AOV) is: $357.92 

VIEW CODE HERE: 

## Question 2: 

For this question you’ll need to use SQL. Follow this link (https://www.w3schools.com/SQL/TRYSQL.ASP?FILENAME=TRYSQL_SELECT_ALL) to access the data set required for the challenge. Please use queries to answer the following questions. Paste your queries along with your final numerical answers below.

1. How many orders were shipped by Speedy Express in total?\
2. What is the last name of the employee with the most orders?\
3. What product was ordered the most by customers in Germany?\

## Answers: 

1. How many orders were shipped by Speedy Express in total? 

   In total, 54 Orders were shipped by Speedy Express.

2. What is the last name of the employee with the most orders?

   Last name is Peacock.

3. What product was ordered the most by customers in Germany? <br/>

   Boston Crab Meat was most ordered by Germany-based customers with a total of 160 orders.
   
VIEW CODE HERE: 
