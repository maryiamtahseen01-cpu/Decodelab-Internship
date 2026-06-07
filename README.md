# Decodelab-Internship
Data Science Internship
# Week 1 – Data Science Internship

## What I worked on this week

This week, I started my data science internship by diving into a cosmetics dataset. The goal was to go through the entire data analysis process – from loading the data to building a simple prediction model.

## The dataset

The dataset has info on **1,472 cosmetic products**. Each product comes with:

- **Product type** (Moisturizer, Cleanser, Sun protect, etc.)
- **Brand** and **product name**
- **Price** and **user rating** (out of 5)
- **Ingredients** list
- **Skin type suitability** – 5 columns indicating if the product works for Combination, Dry, Normal, Oily, or Sensitive skin

## What I did

### 1. Loaded and explored the data
I used pandas to load the CSV file and checked things like:  
- How many rows and columns? → 1472 rows, 11 columns  
- Any missing values? → None  
- Any duplicates? → None  
- What kind of data is in each column?

### 2. Cleaned the data
Luckily, the data was already pretty clean. I just made sure numeric columns were treated as numbers and that there were no empty values.

### 3. Exploratory Data Analysis (EDA)
I looked at summary stats, checked correlations, and noticed that the skin type columns are highly correlated with each other (makes sense – products suitable for normal skin often work for dry skin too).

### 4. Made some plots
- Boxplots to spot outliers  
- Histograms to see how price and ratings are distributed  
- A heatmap to visualize correlations  
- A bar chart showing how many products fall under each type (Moisturizers are the most common)

### 5. Built a prediction model
I tried to predict whether a product is suitable for **sensitive skin** using:
- Price
- Rating
- Suitability for other skin types

I used **Linear Regression**, split the data into training (80%) and testing (20%), and got a **Mean Squared Error of 0.113**.

Here's a peek at how the predictions looked:

| Actual | Predicted |
|--------|-----------|
| 1      | 0.80      |
| 0      | -0.02     |
| 0      | 0.81      |

## Tools I used
- Python
- Pandas & NumPy
- Matplotlib & Seaborn
- Scikit-learn

## Files in this repo
- `Week_1_of_Data_Science_Internship.ipynb` – the full notebook with all my code  
- `cosmatics dataset.csv` – the dataset  
- `README.md` – this file

## What I learned
- This dataset is clean and ready to use  
- Skin type features are closely related  
- Even a simple linear model can give decent predictions  
- Visualizations make it way easier to understand the data  

## What's next?
In Week 2, I plan to try classification models (since I'm predicting a yes/no outcome), do some feature engineering with the ingredients column, and tune the model for better performance.

---

Made with ☕ by a data science intern on a mission 🚀
