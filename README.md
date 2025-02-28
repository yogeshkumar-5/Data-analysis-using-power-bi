# Bank Loan Analysis

## Introduction
This project analyzes bank loan data using **MS SQL Server** and **Power BI** to extract key insights, track loan performance, and optimize lending strategies. It covers loan application trends, funded amounts, borrower risk factors, and regional loan distributions.

## Project Objectives
- Analyze loan application trends and track financial performance.
- Categorize loans as **'Good'** or **'Bad'** based on repayment data.
- Identify regional and employment-based lending patterns.
- Create **interactive dashboards** for real-time insights.

## Tech Stack
- **Database:** Microsoft SQL Server 2022
- **Visualization:** Power BI (February 2025 Version), Tableau (for comparison)
- **Data Processing:** Microsoft Excel 2024

## Project Setup

## Dataset Description
The dataset contains historical bank loan records, including borrower details, loan status, and financial metrics.
- **Columns:** Loan ID, Applicant Income, Loan Amount, Loan Status, Interest Rate, Debt-to-Income Ratio (DTI), Employment Length, etc.
- **Source:** [Specify the source if publicly available]
- **Preprocessing:** Missing values handled, data normalization, outliers removed.  
1. 📝 Clone this repository:  
   ```bash
   git clone https://github.com/your-repo/bank-loan-analysis.git
   ```  
2. 🖥 Install Microsoft SQL Server and SSMS.  
3. 📥 Import the dataset and execute the provided SQL scripts.  
4. 📡 Open Power BI and connect it to the SQL database.  
5. 📊 Load data and explore the dashboards.  

## Data Processing & Analysis
### 1. **MS SQL Server - Data Cleaning & Querying**
- 🛠 **Data Import**: Using MS SQL Server
- 🏗 **Database Creation**
- 📜 **SQL Queries** for Business Problem Solving
- 🧹 **Data Cleaning**: Handling missing values, incorrect data types, duplicates
- ⚡ **Query Optimization**: Using Joins, Aggregate Functions, CTEs, Window Functions

### 2. **Power BI - Data Visualization & Reporting**
#### **Dashboard 1: Summary**
- **KPIs:**
  - 📌 Total Loan Applications (MTD, MoM Tracking)
  - 💰 Total Funded Amount & Amount Received
  - 📉 Average Interest Rate & Debt-to-Income Ratio (DTI)

#### **Dashboard 2: Overview**
- **Key Visuals:**
  - 📆 Monthly Trends (Line Chart)
  - 🌍 Regional Loan Distribution (Map Visualization)
  - 📊 Loan Term Analysis (Donut Chart)
  - 👔 Employment Length vs. Loan Approval (Bar Chart)
  - 💳 Loan Purpose Breakdown (Bar Chart)
  - 🏡 Home Ownership Impact (Tree Map)

#### **Dashboard 3: Loan Details**
- Provides **comprehensive loan insights** 🏦 for decision-makers.
- Enhances transparency with **real-time metrics** 📊.

## Sample SQL Query  
```sql
SELECT loan_status, COUNT(*) AS total_loans
FROM bank_loans
GROUP BY loan_status;
```

## API Integration
- The project integrates with a live financial API to fetch real-time loan interest rates.
- API Endpoint: `https://api.example.com/loans`
- Authentication: API Key-based authentication

## Dashboard Preview  
![Loan Analysis Dashboard](images/dashboard_screenshot.png)  

## Business Insights & Recommendations
- **Loan Performance**: Loans with lower DTI ratios perform better.
- **Regional Trends**: Default rates vary by state; stricter assessments needed.
- **Interest Rate Optimization**: High interest rates correlate with higher defaults.
- **Employment-based Approvals**: Longer job tenure improves repayment rates.

## How to Contribute
1. Fork the repository.
2. Create a new branch: `git checkout -b feature-branch`
3. Make your changes and commit them: `git commit -m "Added new feature"`
4. Push to the branch: `git push origin feature-branch`
5. Open a Pull Request.

## Future Improvements
- Implement **Machine Learning Models** for loan default prediction.
- Integrate **real-time loan data streaming**.
- Enhance **user interactivity** with Power BI reports.

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Author
- **[Your Name]**
- **[Your Contact Info]**
