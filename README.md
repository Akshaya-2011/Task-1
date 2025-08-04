# Task-1

 Dataset Summary: Amazon Sale Report
About the Dataset:
Contains 128,975 rows and 24 columns.

Tracks order details from Amazon.in such as:

Order ID, Date, Status, Category, Amount, Shipping details, etc.

Used for analyzing sales, returns, delivery performance, and product trends.

 Cleaning Performed:
🔸 Step 1: Loaded the Dataset Safely
Skipped any bad or broken lines using on_bad_lines='skip'.

Prevented quote issues and column type warnings.

🔸 Step 2: Removed Unnecessary Columns
Dropped Unnamed: 22 and fulfilled-by (mostly empty or not useful).

🔸 Step 3: Converted Data Types
Converted the Date column from text to datetime format for time-based analysis.

🔸 Step 4: Handled Missing Values
Dropped rows with missing Amount or currency — these are critical.

Filled other missing columns:

Courier Status → "Unknown"

promotion-ids → "None"

ship-city, ship-state, ship-country → "Unknown"

ship-postal-code → 0

🔸 Step 5: Reset and Save
Reset the index to make the data clean and continuous.

Saved as Cleaned_Amazon_Sale_Report.csv.

✅ Final Dataset:
Cleaned rows: 121,180
