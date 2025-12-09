📊 Website Performance Analysis Report

Time Period: April – May 2024
Dataset: watching_customer.csv
Rows: 3,182 observations


1. Dataset Overview
This dataset contains hourly performance metrics of a website across various acquisition channels.
Key Metrics Included
Users
Sessions
Engaged Sessions
Average Engagement Time per Session
Events per Session
Engagement Rate
Event Count
Channel Group (Direct, Organic Social, Organic Search, Email, Referral, etc.)
DateHour (YYYYMMDDHH → converted to datetime)
Hour extracted for time-based analysis

2. Data Cleaning & Preprocessing
Steps performed before analysis:
Removed an incorrect header row inside the data
Standardized all column names
Converted DateHour string (YYYYMMDDHH) → proper datetime format
Converted all numeric columns from string to numeric types
Extracted Hour of Day for trend analysis
Handled missing values and ensured clean datatypes for visualizations

📈 3. Key Insights
🔹 A. Time Trends
Clear daily and weekly seasonality in Users & Sessions
Peak traffic during business hours and weekdays
Stable overall trend without major anomalies

🔹 B. Channel Performance
User Acquisition
Organic Social and Organic Search contribute the highest user volume.
Engagement Time
Direct channel shows the highest engagement (~200–250 seconds).
Organic Social has shorter session durations (~30–50 seconds).
Engagement Rate
Most channels show 0.4–0.6 engagement rate (low variance).
Direct and Email have slightly higher median engagement rates.

🔹 C. Engaged vs Non-Engaged Sessions
Engaged sessions form a major share across channels.
Direct and Organic Search show the highest engaged-session volume.

🔹 D. Hourly Traffic Patterns / Heatmap
Highest activity: 18:00–22:00 (evening peak)
Lowest activity: 00:00–06:00
Organic Social & Direct dominate peak-hour traffic
Email & Referral show lower but consistent traffic throughout the day

🔹 E. Engagement Rate vs Sessions
Mild inverse relationship at times – high traffic spikes → lower engagement
Overall engagement rate remains stable around 40–50%

🛠️ 4. Tools & Technologies Used
Python Pandas, NumPy for data cleaning
Matplotlib, Seaborn for visualization
Jupyter Notebook for analysis workflow

📄 5. How to Use This Project
Clone the repository
Install the required Python libraries
Open the Jupyter Notebook
Run the cells to reproduce all charts and insights

📌 6. Future Improvements
Add anomaly detection
Build a forecasting model
Include deeper channel attribution analysis
