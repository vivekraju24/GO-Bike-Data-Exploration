# GO-Bike-Data-Exploration
## **Ford GoBike System Data Exploration and Findings Communication**  
This document analyzes a dataset containing details of individual rides in a bike-sharing system operating in the greater San Francisco Bay Area in 2019.  

### **Dataset**  
The dataset includes **183,412 rides** and contains **16 features**, which include:  
- `'duration_sec'`, `'start_time'`, `'end_time'`, `'start_station_id'`, `'start_station_name'`, `'start_station_latitude'`, `'start_station_longitude'`,  
- `'end_station_id'`, `'end_station_name'`, `'end_station_latitude'`, `'end_station_longitude'`, `'bike_id'`, `'user_type'`,  
- `'member_birth_year'`, `'member_gender'`, `'bike_share_for_all_trip'`.  

After data cleaning and transformation, the dataset was refined into **11 features**, introducing new columns:  

- **`day_of_week`**: Extracted weekday number from `start_time`.  
- **`start_hour`**: Extracted hour number from `start_time`.  
- **`time_of_day`**: Categorized from `start_hour` to represent the time of day.  
- **`duration_min`**: Converted `duration_sec` into minutes.  
- **`user_age`**: Derived from `member_birth_year`.  
- **`user_age_bin`**: Grouped ages into bins for demographic analysis.  

---

### **Summary of Findings**  
Differences in bike usage were observed between **subscribers** and **customers**:  

- **Trip Frequency**:  
  - **Thursday had the highest number of rides**, independent of user type.  
  - **Subscribers** primarily used bikes on **weekdays (Monday–Friday)**.  
  - **Customers’ usage was steady throughout the week**, with a significant increase on **Saturdays and Sundays**.  

- **Trip Duration**:  
  - **Subscribers' trips averaged between 10-11 minutes**, while **customers' trips lasted around 23-24 minutes**.  
  - **Customers were more likely to take trips lasting over an hour compared to subscribers**.  

- **Time of Day Patterns**:  
  - **Subscribers** primarily started trips in the **morning (8 AM) and evening (5 PM)**.  
  - **Customers** preferred riding in the **afternoon**, with peak trips at **5 PM**.  

- **Weekend Trends**:  
  - On average, **weekend trips (Saturday & Sunday) lasted longer than weekday trips**.  

---

### **Key Insights for Presentation**  
For the presentation, the focus was on:  
- **Identifying the most active time of day and day of the week for rides**.  
- **Analyzing the average trip duration for different user types**.  
- **Assessing whether trip duration patterns vary between subscribers and customers**.  

The findings confirmed that:  
- **Customers consistently had longer rides than subscribers across all days and times**.  
- **Subscribers' usage aligned with commuting hours, whereas customers preferred afternoon rides**.  

---

### **Feedback**  
For any feedback or suggestions, feel free to reach out at **vivekraju.24@outlook.com**.  
