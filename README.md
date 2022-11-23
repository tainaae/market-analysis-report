
# market-analysis-report

<p>The Market Analysis Report presents tools and insights related to customer demographics, marketing condition in the USA and products info. It was composed of 5 pages:<br></p>
- Average Income Household by State, which presents a bubble map visual with Income Regional Distribution.
- Income and Sales Correlation, which presents a scatter plot visual that shows the relationship between Average Sales and Average Income by State.
- Products and Customers Profiles, with 2 visuals: a multi-row card that shows customer rating and current price per product, and a histogram that presents the Average Purchases per Income Range.
- Customers Demographics, with a scatter plot visual that was used to determine the correlation between the size of a population and the average income by state.
- Product Insights, with a scatter plot visual that was used to determine the correlation between the average customer rating and the average return rating per product.<br>
<p>The core of the analysis is the linear regression built from Income by State and 6 Months Sales that was used to predict customer income (y) from customer sales (x).</p>
y=0.01x-722.14
<p>From the regression formula, a calculated column was created with predicted customers income based on their total purchases and the customer that is predicted to have the highest income was found: Jon Little (JLit30836), from Illinois. After that, the measure of the correlation (R2 value) between sales and income returns the value of 0.78, indicating a strong positive relationship between the two variables.</p>
<p>The correlation between population size and average income by state was also calculated and the result of correlation of 0.04 indicated that there is a low to no dependency between the variables. From that, it was possible to conclude that the size of population doesn't impact much in average income of a state’s population.</p>
<p>The information retrieved from products data was used to calculate the correlation (R2 value) between customer ratings and product return rate, which resulted in a negative correlation between these variables, telling us that the highest the product customer rating, there is a great chance that the return rate of same product being low./<p>
<p>Though there is no way of recommending specific clothing styles by region based on the available data, it is possible to associate products with purchasing power and purchasing trends per State. To do that, a calculated column was added by the ‘Customer List’, where the product recommendations was defined using a DAX formula that groups products per income range, as represented in the table below:</p>
Income Range	Product Price Range
Less than $90,000	$0 - $50
Between $90,000 and $160,000	$50 - $100
Between $160,000 and $195,000	$100 - $200
Between $195 and $265,000	$200 - $350
Between $265,000 and $335,000	$350 - $700
Greater than $335,000	$700 - $1100

<p>For instance, the Spring T-shirts, Cotton Sweater and Leather Bag’ current prices are, respectively,  $25, $100, $1000 so they are recommended for customers who fit in the Less than $90,000, Between $90,000 and $160,000 and Greater than $335,000 ranges.</p>
