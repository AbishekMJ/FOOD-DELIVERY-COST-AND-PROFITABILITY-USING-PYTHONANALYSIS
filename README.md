# FOOD-DELIVERY-COST-AND-PROFITABILITY-ANALYSIS-USING-PYTHON
 A data-driven analysis of food delivery operations to evaluate costs, revenue, and profitability, and to recommend strategies for improving financial performance using python

#### Overview
This project is aimed at understanding the financial dynamics of food delivery operations by analyzing order data to determine costs, revenues, and profitability. It uses Python libraries such as `pandas`, `matplotlib`, and `seaborn` to provide insights into the financial performance and suggest strategies for improvement.

The food delivery industry has seen significant growth, especially with the advent of online ordering platforms. With this growth, understanding the economics of food delivery has become crucial for both restaurants and delivery platforms. The aim of this project is to analyze the various cost components and profitability of food delivery orders from restaurants in New Delhi. The analysis focuses on understanding how different factors, such as discounts, commissions, and delivery fees, impact the overall profitability of these transactions.

This project involves analyzing food delivery orders from restaurants in New Delhi. The analysis focuses on understanding the impact of discounts and commission fees on profitability. It calculates actual profits, simulates profits under recommended commission and discount rates, and compares these metrics. The project includes data preprocessing, descriptive analysis, and visualization to provide insights into revenue, costs, and profitability.

## ABOUT DATASET

The dataset contains records of food delivery orders in New Delhi, with the following key columns:
	Order ID: A unique identifier for each order.
	Customer ID: The unique identifier for the customer who placed the order.
	Restaurant ID: The unique identifier for the restaurant fulfilling the order.
	Order Date and Time: The timestamp when the order was placed.
	Delivery Date and Time: The timestamp when the order was delivered.
	Order Value: The total monetary value of the order (in INR).
	Delivery Fee: The fee charged to the customer for delivering the order.
	Commission Fee: The fee charged by the platform to the restaurant for facilitating the order.
	Payment Processing Fee: The fee incurred for processing the customer's payment.
	Refunds/Chargebacks: Any amounts refunded to the customer or chargebacks applied.
	Discounts and Offers: Discounts or promotional offers applied to the order.
	Discount Percentage/Flat Off: A breakdown of the type and value of discounts applied.
	Discount Amount: The total amount of money discounted from the order.
	Total Costs: The sum of all costs associated with the order, including fees and discounts.
	Revenue: The revenue generated from the commission fee.
	Profit: The net profit after subtracting total costs from revenue.
The dataset is used to calculate various metrics related to order profitability, such as the impact of discounts and commissions.

### GOAL OF PROJECT

The project involves analyzing the profitability of food delivery orders by first preprocessing the dataset to handle missing values, extract discount types, and calculate discount amounts. Total costs are then computed by adding delivery fees, payment processing fees, and discount amounts, while profit is derived from subtracting these costs from revenue. The analysis includes exploring the distribution of profits and breaking down costs into components such as delivery fees and discounts. Simulations are conducted to estimate profitability under adjusted commission and discount rates. Visualizations, including histograms and KDE plots, are used to compare actual and simulated profitability. The findings help identify optimal commission and discount strategies to enhance overall profitability without compromising customer satisfaction.


#### Project Description

Data Processing

1. Data Loading:
   - The project starts by importing a CSV file containing food order data.
   - The data is processed to convert relevant columns into date formats and set these columns as indices to facilitate easier manipulation.

2. Discount Handling:
   - Discounts and offers are normalized into a consistent numeric format. 
   - Discounts are categorized into two types: percentage-based and flat amounts, and then converted into numeric values for accurate calculations.

3. Cost Calculation:
   - Total costs are calculated by summing up the delivery fees, payment processing fees, and discount amounts for each order.
   - Revenue is computed based on the commission fees collected.
   - Profit is determined by subtracting the total costs from the revenue.

**Analysis**

1. Cost and Profit Metrics:
   - Total costs, revenue, and profit are aggregated to gauge the overall financial performance.
   - Metrics are analyzed to understand how costs and revenues balance out and to identify areas for improvement.

2. Visualizations:
   - Profit Distribution Histogram: Displays the distribution of profit per order, highlighting the number of orders that are profitable versus those that are not.
   - Costs Breakdown Pie Chart: Illustrates the proportion of total costs allocated to delivery fees, payment processing fees, and discounts.
   - Revenue vs. Costs Bar Chart: Compares total revenue, total costs, and total profit to show the financial gap and overall profitability.

3. New Strategy for Profitability:
   - The analysis of profitable orders helps to determine effective commission and discount rates.
   - Simulations are run to see how adjusted rates could impact profitability, comparing these results with actual figures to suggest improvements.

#### Results

Current State:
- The analysis shows that total costs exceed revenue, resulting in a net loss. This indicates that the current commission rates, delivery fees, and discount strategies are not sufficient for profitability.

Recommended Strategy:
- To improve profitability, a commission rate of 28% and a discount rate of 6% are suggested based on the analysis.

Simulation Results:
- Simulations with the recommended rates indicate a potential improvement in profitability. Revenue surpasses costs with these adjusted rates, suggesting a more sustainable financial model.

#### Getting Started

Prerequisites:
- Ensure you have Python libraries installed: `pandas`, `matplotlib`, and `seaborn`. You can install them using `pip`.

**Running the Analysis:**
1. Download the Dataset: Place your dataset file (e.g., `food_orders_new_delhi.csv`) in the project directory.
2. Execute the Code: Run the provided Python script to process the data, perform calculations, and generate visualizations.
3. Review Results: Check the console for summary statistics and review the generated plots for visual insights into cost, revenue, and profitability.

#### Contributing
Contributions to improve the analysis or extend its functionality are welcome. Please follow these steps for contributions:
1. Fork the repository.
2. Create a new branch.
3. Commit your changes.
4. Open a pull request.

#### License
This project is licensed under the MIT License. See the LICENSE file for details.

#### Contact
For any questions or feedback, please contact [abishekmjabishekmj1569@gmail.com].
