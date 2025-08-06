# 📊 Mobile Sales Insights Dashboard - Power BI Project

## 📁 Project Overview
The Mobile Sales Insights Dashboard is an interactive Power BI report designed to provide a comprehensive analysis of mobile sales performance across cities, mobile models, payment methods, and customer behaviors. This dashboard enables businesses to identify sales trends, optimize inventory, and make informed strategic decisions.

## 🎯 Problem Statement
The organization requires a centralized and visually appealing dashboard to:
- Monitor sales KPIs at a glance
- Analyze sales distribution across cities and time periods
- Identify top-selling mobile models and preferred payment methods
- Understand customer preferences through ratings and buying behavior
- Provide dynamic filters for in-depth data exploration

## 📝 Purpose of Dashboard
- Track overall Sales Performance & KPIs
- Visualize Sales Distribution across Cities & Time Periods
- Identify Top-Selling Mobile Models and Payment Preferences
- Analyze Customer Ratings & Buying Patterns
- Enable Interactive Filtering by Model, Brand, Payment Method, and Date

## 📊 Key KPIs & Metrics
1. Total Sales (₹)
2. Total Quantity Sold (Units)
3. Total Transactions (Count)
4. Average Price per Unit (₹)
5. Sales by City
6. Sales by Mobile Model (Top 3)
7. Sales by Day Name (Mon-Sun)
8. Units Sold vs Price by Brand
9. Transactions by Payment Method
10. Customer Ratings Distribution (1-5 Stars)

## 📈 Visualizations in Dashboard
- **Cards**: Total Sales, Quantity Sold, Transactions, Average Price per Unit
- **Map Chart**: Total Sales by City (Bubble Size by Sales Value)
- **Line Chart**: Total Quantity Sold by Month
- **Column Chart**: Top 3 Mobile Models by Total Sales
- **Pie Chart**: Transactions Distribution by Payment Method
- **Funnel Chart**: Customer Ratings Distribution (1 to 5 Stars)
- **Area Chart**: Total Sales by Day Name
- **Scatter Chart**: Units Sold vs Price per Unit by Brand

## 🛠️ Steps to Build the Dashboard

### Step 1: Import Data
- Import Mobile Sales Data into Power BI
- Validate fields: Date, Brand, City, Mobile Model, Units Sold, Total Sales, Price per Unit, Transactions, Ratings, Payment Method

### Step 2: Data Transformation (Power Query)
- Set correct Data Types (Date, Currency, Whole Numbers, Text)
- Extract Month Name & Day Name from Date
- Remove unnecessary columns

### Step 3: UI Customization
- Import Mobile Icon/Logo and place it at the Top-Left Corner
- Set a Light Cyan/Teal Background Theme
- Use Rectangles/Shapes for layout sections:
  - Left Sidebar (Filters/Slicers)
  - Top KPI Cards
  - Main Chart Area

### Step 4: Slicers
- Add a Month Name Slicer (Single Select Mode)
- Add Dropdown Slicers for:
  - Mobile Model
  - Brand
  - Payment Method
  - Day Name
    
### Step 5: Create DAX Measures
- Total Sales = SUMX('Mobile Sales Data', 'Mobile Sales Data'[Units Sold] * 'Mobile Sales Data'[Price Per Unit])
- Total Quantity = SUM('Mobile Sales Data'[Units Sold])
- Total Transactions = COUNTROWS('Mobile Sales Data')
- Average Price = AVERAGE('Mobile Sales Data'[Price Per Unit])

### Step 6: Visualization Implementation
- Cards for KPIs (Total Sales, Quantity, Transactions, Average Price)
- Map Chart for Total Sales by City (Bubble Size = Total Sales, Style = TomTom)
- Line Chart for Quantity Sold by Month (with Data Labels)
- Column Chart for Top 3 Mobile Models (Apply Top N Filter)
- Pie Chart for Transactions by Payment Method (with Percentage Labels)
- Funnel Chart for Customer Ratings Distribution (Sorted Descending)
- Area Chart for Total Sales by Day Name (Sorted Mon-Sun)
- Scatter Chart for Units Sold vs Price per Unit (Size = Total Sales, Legend = Brand, Details = Model)

## 🖥️ Tools & Technologies Used
- Microsoft Power BI Desktop
- Power Query Editor
- DAX (Data Analysis Expressions)
- TomTom Map Visuals
- Custom Icons/Images

## 🚀 Outcome & Impact
- Real-time insights into sales trends across various dimensions
- Data-driven decisions for inventory planning & marketing strategies
- Improved visibility into customer preferences and payment behavior
- Enhanced business performance tracking through interactive visualizations

## 📌 Notes
- Ensure data is refreshed periodically for up-to-date analysis
- Adjust chart colors and themes as per brand guidelines if required
- Apply necessary filters on slicers to avoid cluttered visualizations

## 📧 Contact
For any queries or customization support:  
**Chavi Jain**  
📩 chavijain2303@gmail.com 


