# 🗽 NYC Airbnb Data Analysis

Welcome to this exploratory data analysis project focused on Airbnb listings in New York City. The main goal of this notebook is to uncover insights about pricing, availability, guest preferences, and outliers, while also building a clear understanding of how Airbnb operates across different neighborhoods in NYC.

---

## 📦 Dataset

- Source: [Inside Airbnb](https://insideairbnb.com/get-the-data.html)
- File used: `listings.csv` — containing summary information about each listing
- Entries: 37,541
- Features: 18

---

## 🔍 Objectives

- Understand distribution of room types and price ranges
- Analyze missing data and variable types
- Detect and handle outliers in price and minimum nights
- Explore guest behavior and host patterns
- Identify trends by neighborhood and borough
- Clean and reshape the dataset for meaningful insights

---

## 🧹 Data Cleaning Highlights

- Removed irrelevant variables like `license` (85% missing)
- Handled missing data in `reviews_per_month` and `last_review`
- Cleaned outliers in:
  - `minimum_nights` (filtered to stays under 180 days)
  - `price` (filtered to listings priced under $1000)

---

## 📊 Key Insights

### 🛏️ Most Common Room Types
- Entire home/apartment: **52.8%**
- Private room: **44.6%**

### 💵 Price by Borough
| Borough        | Average Price (USD) |
|----------------|---------------------|
| Manhattan      | 259.58              |
| Brooklyn       | 160.08              |
| Queens         | 126.56              |
| Staten Island  | 122.55              |
| Bronx          | 118.24              |

### 🏘️ Most Expensive Neighborhoods (based on average price)
- Rossville (Staten Island)
- Fort Wadsworth (Staten Island)
- NoHo, SoHo, Tribeca, Battery Park (Manhattan)

⚠️ Note: Some outliers affected the ranking of neighborhoods, such as extremely high-priced listings in less popular areas. This was later validated by analyzing the number of listings per neighborhood.

---

## 📌 Observations

- **Minimum nights** often defaults to 30, possibly due to platform rules or host preferences.
- A small portion of users (5.8%) book for over 30 days — possibly students or professionals on mid-term stays.
- A handful of listings had extremely high prices or minimum stay requirements — these were considered outliers and excluded.

---

## 🛠️ Tools Used

- Python
- Pandas
- NumPy
- Matplotlib / Seaborn
- Google Colab

---

## ✍️ Author

Project by [Your Name]  
Built as part of a hands-on learning journey in Data Science and exploratory analysis.

---

## 📎 License

This project is for educational and personal learning purposes only.
