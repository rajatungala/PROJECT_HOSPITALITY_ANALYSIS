

# AtliQ Hotels Data Analysis Project

## Overview
This project focuses on analyzing booking data for AtliQ Hotels to derive actionable insights about revenue, customer behavior, and operational performance. The analysis is conducted using Python with libraries such as Pandas, and the results are presented in a Jupyter Notebook. The dataset includes information about hotel bookings, properties, room categories, and dates, spanning multiple cities in India.

## Project Structure
- **Notebook**: `AtliQ_Hotels_Data_Analysis.ipynb` - The main Jupyter Notebook containing the data analysis code and visualizations.
- **Datasets**:
  - `dim_date.csv`: Contains date-related information (e.g., month, week number, day type).
  - `dim_hotels.csv`: Details about hotel properties (e.g., property ID, name, category, city).
  - `dim_rooms.csv`: Information about room categories.
  - `fact_aggregated_bookings.csv`: Aggregated booking data.
  - `fact_bookings.csv`: Detailed booking records (e.g., booking ID, dates, revenue, status).
- **Outputs**: Visualizations and results are embedded in the notebook (e.g., pie charts, tables).

## Objectives
1. **Data Exploration**: Understand the structure and contents of the datasets.
2. **Revenue Analysis**:
   - Revenue realized per city.
   - Month-by-month revenue trends.
   - Revenue by hotel type .
3. **Customer Insights**:
   - Average ratings per city 
   - Distribution of revenue across booking platforms .
4. **Data Cleaning**: Handle anomalies like negative guest numbers and outliers in revenue.

## Tools and Technologies
- **Python**: Core programming language.
- **Pandas**: Data manipulation and analysis.
- **Matplotlib/Seaborn**: Visualization (for pie charts and other plots).
- **Jupyter Notebook**: Interactive environment for analysis and documentation.

## Installation
To run this project locally, follow these steps:

1. **Clone the Repository**:
   ```bash
   git clone https://github.com/your-username/atliq-hotels-data-analysis.git
   cd atliq-hotels-data-analysis
   ```

2. **Set Up a Virtual Environment** (optional but recommended):
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. **Install Dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
   Open `AtliQ_Hotels_Data_Analysis.ipynb` in your browser.

## Requirements
Ensure the following Python packages are installed:
```plaintext
pandas
matplotlib
seaborn
jupyter
```
You can install them using:
```bash
pip install pandas matplotlib seaborn jupyter
```

## Usage
1. Place the datasets (`dim_date.csv`, `dim_hotels.csv`, `dim_rooms.csv`, `fact_aggregated_bookings.csv`, `fact_bookings.csv`) in a `datasets/` folder within the repository.
2. Open the Jupyter Notebook and run the cells sequentially to:
   - Load and explore the data.
   - Perform data cleaning and merging.
   - Generate insights and visualizations.
3. Complete the exercises (revenue per hotel type, average rating per city, pie chart of revenue by platform) by adding your code in the designated sections.

## Key Insights
- **Revenue by City**: Mumbai leads with the highest revenue realized (668,569,251), followed by Bangalore, Hyderabad, and Delhi.
- **Monthly Revenue**: May 2022 had the highest revenue (408,375,641), followed by July and June.
- **Booking Platforms**: "Others" is the most used platform (55,066 bookings), followed by "makeyourtrip" and "logtrip".
- **Room Categories**: Four types (RT1, RT2, RT3, RT4) are available across the hotels.

## Exercises
The notebook includes three exercises for further analysis:
1. **Revenue Realized per Hotel Type**: Group by `category` (e.g., Luxury, Business) and sum `revenue_realized`.
2. **Average Rating per City**: Group by `city` and calculate the mean of `ratings_given`.
3. **Pie Chart of Revenue by Booking Platform**: Use `booking_platform` and `revenue_realized` to visualize the distribution.

## Data Cleaning Notes
- Negative `no_guests` values (e.g., -3, -2) were observed and should be filtered or corrected.
- Outliers like `revenue_generated` of 9,100,000 indicate potential data entry errors.
- Date formats were standardized using `pd.to_datetime` for consistency.





