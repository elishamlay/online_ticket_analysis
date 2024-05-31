# Online Ticket System Data Analysis Project

## Project Overview
This project involves analyzing data from an online ticket system for the year 2024. The analysis aims to uncover insights related to sales performance, customer segmentation, revenue trends, and more. The findings will help in understanding customer behavior, optimizing pricing strategies, and identifying peak sales periods.

## Table of Contents
1. [Data Collection](#data-collection)
2. [Data Preparation](#data-preparation)
3. [Data Analysis](#data-analysis)
    - [Sales Analysis by Event Type](#sales-analysis-by-event-type)
    - [Customer Segmentation](#customer-segmentation)
    - [Revenue Trends Over Time](#revenue-trends-over-time)
    - [Additional Analyses](#additional-analyses)
4. [Conclusion](#conclusion)
5. [Usage](#usage)
6. [Files](#files)

## Data Collection
The dataset was generated using the `Faker` library in Python. It includes synthetic data for ticket transactions that occurred throughout 2024. The dataset contains the following columns:
- `TransactionID`: Unique identifier for each transaction
- `DateTime`: Date and time of the transaction
- `EventType`: Type of the event (e.g., Concert, Sports, Theater)
- `TicketPrice`: Price of the ticket
- `QuantitySold`: Number of tickets sold in the transaction
- `CustomerID`: Unique identifier for each customer
- `CustomerAge`: Age of the customer
- `CustomerGender`: Gender of the customer
- `CustomerLocation`: Location of the customer

## Data Preparation
1. **Loading the Data**: The dataset is loaded into a pandas DataFrame.
2. **Cleaning the Data**: The data is checked for any missing or inconsistent values. Any necessary data transformations are applied to ensure consistency.
3. **Feature Engineering**: New features, such as age groups, are created to aid in analysis.

## Data Analysis
### Sales Analysis by Event Type
- **Objective**: Understand revenue distribution across different event types.
- **Method**: Aggregate total revenue, average ticket price, and total quantity sold for each event type.
- **Results**: Insights into which event types generate the most revenue and have the highest average ticket prices.

### Customer Segmentation
#### Age Group Segmentation
- **Objective**: Categorize customers into age groups and analyze their distribution.
- **Method**: Use pandas `cut` function to create age groups.
- **Results**: Distribution of customers across different age groups.

#### Gender Segmentation
- **Objective**: Analyze the gender distribution among customers.
- **Method**: Count the number of male and female customers.
- **Results**: Insights into gender composition of the customer base.

#### Location Segmentation
- **Objective**: Understand where most customers are located.
- **Method**: Count the number of transactions from each location.
- **Results**: Geographic distribution of customers.

### Revenue Trends Over Time
- **Objective**: Identify revenue patterns and seasonal trends.
- **Method**: Resample data monthly and plot total revenue.
- **Results**: Visualization of revenue trends over the year.

### Additional Analyses
#### Customer Loyalty Analysis
- **Objective**: Identify repeat customers and analyze loyalty.
- **Method**: Count the number of transactions per customer.
- **Results**: Percentage of customers with multiple transactions.

#### Event Type Preference by Age Group
- **Objective**: Understand event type preferences among different age groups.
- **Method**: Group data by age group and event type.
- **Results**: Insights into which age groups prefer certain event types.

## Conclusion
The analysis provided valuable insights into sales performance, customer demographics, and revenue trends. These insights can inform strategic decisions in marketing, event planning, and customer engagement.

## Usage
To replicate the analysis:
1. Ensure you have Python and the necessary libraries installed (`pandas`, `matplotlib`, `faker`).
2. Load the dataset using `pd.read_csv('path/to/ticket_sales_2024.csv')`.
3. Run the provided analysis scripts to generate insights and visualizations.

## Files
- `ticket_sales_2024.csv`: The dataset containing ticket sales data.
- `analysis_script.py`: Python script containing the data analysis code.
- `visualizations/`: Directory containing generated visualizations.
