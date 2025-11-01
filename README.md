## Author
**Name:** Mufiz Arbee  

---

## 📘 Summary / Approach

This project performs **end-to-end retail data analysis** by integrating data from transactions, customers, and product catalogs.  
The workflow focuses on **data cleaning, feature engineering, customer-level insights, and monthly performance metrics** using fully **vectorized operations** for efficiency.

### **Core Steps:**
1. **Data Loading & Inspection**  
   - Loaded and inspected `transactions.csv`, `customers.csv`, and `products.csv`.  
   - Checked for missing values and data inconsistencies.

2. **Data Cleaning & Preprocessing**  
   - Handled missing numeric values using the median and categorical values using the mode.  
   - Converted timestamps to datetime and extracted features like hour, day, and month.

3. **Feature Engineering**  
   - Calculated derived metrics: `revenue = quantity × price` and `profit_margin`.  
   - Created time-based and aggregated features such as `month_year`.

4. **Data Integration**  
   - Merged all datasets (`transactions`, `customers`, `products`) into a unified `full_data` frame.

5. **Customer Metrics**  
   - Computed total revenue, number of transactions, average order value, and most frequent purchase category per customer.

6. **Monthly Metrics**  
   - Aggregated key metrics by month, including revenue growth percentage and average order value.

7. **Duplicate Detection (Advanced Task)**  
   - Identified potential duplicate customers based on fuzzy name matching, email domain similarity, and transaction overlap.

---

## ⚙️ Dependencies / Libraries Used

| Library | Purpose |
|----------|----------|
| **pandas** | Data manipulation, aggregation, and time-series operations |
| **numpy** | Mathematical operations and vectorization |
| **fuzzywuzzy** | String similarity matching for duplicate detection |
| **scikit-learn** | Optional helper functions for text/vector comparison |
| **datetime** | Timestamp handling and date arithmetic |
| **time** | Benchmarking performance of vectorized vs loop operations |

---
