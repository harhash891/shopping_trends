# Shopping Trends Analysis

This repository contains an exploratory data analysis (EDA) of a retail shopping dataset. The analysis is performed in a Jupyter Notebook (`n1.ipynb`) using Python and popular data science libraries.

## Dataset

The dataset `shopping_trends.csv` includes customer purchase records with the following columns:

- **Customer ID** – unique identifier  
- **Age** – customer age  
- **Gender** – Male/Female  
- **Item Purchased** – product name  
- **Category** – product category (Clothing, Footwear, Accessories, Outerwear)  
- **Purchase Amount (USD)** – transaction value  
- **Location** – US state  
- **Size** – clothing size (S, M, L, XL)  
- **Color** – product color  
- **Season** – season of purchase  
- **Review Rating** – customer rating (2.5–5.0)  
- **Subscription Status** – Yes/No (converted to 1/0)  
- **Payment Method** – method used (e.g., Credit Card, PayPal, Cash)  
- **Shipping Type** – shipping speed  
- **Discount Applied** – Yes/No (converted to 1/0)  
- **Promo Code Used** – Yes/No (converted to 1/0)  
- **Previous Purchases** – number of prior purchases  
- **Preferred Payment Method** – customer’s preferred method  
- **Frequency of Purchases** – purchase frequency (Weekly, Monthly, Quarterly, etc.)

## Analysis & Visualizations

The notebook performs the following steps:

1. **Data loading & preprocessing**  
   - Convert Yes/No columns to binary (1/0).

2. **Descriptive statistics**  
   - Summary statistics for numerical columns.

3. **Customer age distribution**  
   - Histogram of customer ages.

4. **Gender distribution**  
   - Pie chart showing proportion of male/female customers.

5. **Average purchase amount by category**  
   - Grouped bar chart – Footwear has the highest average purchase amount.

6. **Purchase amount by payment method**  
   - Grouped bar chart – Credit Card and Venmo show higher average amounts.

7. **Purchase amount by season**  
   - Total purchase amount per season – Fall leads, followed by Spring, Winter, Summer.

8. **Purchase amount by size**  
   - Average purchase amount per size – S slightly higher than others.

9. **Review rating by discount applied**  
   - Maximum rating is 5.0 regardless of discount.

10. **Previous purchases frequency**  
    - Median previous purchases by purchase frequency.

11. **Color & category relationships**  
    - Cross-tabulation of color and category.

12. **Pivot table**  
    - Average purchase amount by location and item purchased.

13. **Boxplots**  
    - Purchase amount distribution by frequency of purchases.

14. **Correlation analysis**  
    - Scatter plots and heatmaps (not heavily used, but some relationships explored).

## Key Findings (Summary)

- **Average purchase amount**: Highest for Footwear (~$60.26), followed by Clothing (~$60.03).
- **Gender split**: Nearly equal proportion of male and female customers.
- **Age distribution**: Majority of customers between 30–60 years old.
- **Payment methods**: Credit Card and PayPal are most preferred; Venmo also popular.
- **Seasonal spending**: Fall generates the highest total revenue.
- **Discounts**: Discounts do not significantly impact maximum review ratings.
- **Purchase frequency**: Weekly buyers tend to have higher median previous purchases.

## Requirements

The notebook uses the following Python libraries:

- `pandas`
- `numpy`
- `matplotlib`
- `seaborn`

Install dependencies with:

```bash
pip install pandas numpy matplotlib seaborn
