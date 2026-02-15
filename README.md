# 🏥 Healthcare Analytics Dashboard - Power BI

A comprehensive healthcare analytics solution built with Power BI, featuring advanced data transformation, interactive dashboards, and strategic insights for healthcare operational performance and revenue forecasting.

![Dashboard Overview](screenshots/healthcare_operational_overview.png)

## 📊 Project Overview

This project analyzes healthcare data from 54,966+ patient records to provide actionable insights into:
- Patient demographics and medical conditions
- Billing trends and revenue forecasting
- Operational performance metrics
- Resource utilization and capacity planning
- Risk analysis and strategic recommendations

## ✨ Key Features

### Dashboard 1: Healthcare Operational Performance Overview
- **KPI Cards**: Average stay (15.5 days), Average age (51.54), Total admissions (40.235K), Average bill ($25.59K)
- **Cost Analysis**: High-cost "pockets" identification across medical conditions
- **Trend Analysis**: Medical condition admissions over years (2019-2024)
- **Insurance Analytics**: Admission type distribution by insurance provider
- **Demographics**: Average stay by patient age group and gender
- **Interactive Filters**: Medical condition, admission type, and gender filters

### Dashboard 2: Strategic Revenue Forecasting & Risk Analysis
- **Financial Snapshot**: Total billing ($1.40B), Average invoice ($25.6K), Top provider insights
- **Clinical Trends**: Revenue stability analysis and seasonal volatility assessment
- **Resource Forecasting**: 6-month patient volume predictions and staffing recommendations
- **Time Series Analysis**: Billing amount trends by quarter (2020-2026 forecast)
- **Advanced Filters**: Gender, blood type, medical condition, and age group segmentation

## 🛠️ Technology Stack

- **Power BI Desktop** - Data visualization and dashboard creation
- **Power Query** - Data transformation and cleaning
- **DAX** - Advanced calculations and measures
- **CSV** - Source data format



## 🔄 Data Transformation Process

### Power Query Transformations Applied:

1. **Data Type Corrections**
   - Converted date columns to proper DateTime format
   - Ensured numeric fields (Billing Amount, Age, Room Number) have correct data types
   - Standardized text fields (Name, Gender, Medical Condition)

2. **Data Cleaning**
   - Removed duplicate records
   - Handled missing values
   - Standardized categorical values (Gender, Blood Type, Medical Condition)
   - Validated date ranges (Admission Date vs Discharge Date)

3. **Feature Engineering**
   - Calculated Length of Stay (Days) from admission and discharge dates
   - Created age group categories (Child, Young Adult, Middle Aged, Senior)
   - Generated quarter and year columns for time-series analysis
   - Added billing status categories (Normal, Abnormal, Inconclusive)

4. **Data Validation**
   - Ensured referential integrity across related fields
   - Validated billing amounts against industry standards
   - Cross-checked insurance provider data consistency

## 📈 Key Insights & Findings

### Financial Analysis
- **Total Billing**: $1.40B across all patient records
- **Average Invoice**: $25.6K per patient admission
- **Top Provider**: Cigna (20% of revenue)
- **Revenue Stability**: No significant seasonal volatility observed

### Clinical Trends
- **High-Cost Conditions**: 
  - Diabetes: $236.5M
  - Obesity: $236.0M
  - Arthritis: $235.2M
  - Hypertension: $233.4M
  - Asthma: $233.1M
  - Cancer: $229.9M

### Operational Metrics
- **Average Stay**: 15.5 days
- **Patient Demographics**: Average age 51.54 years
- **Total Admissions**: 40,235 patients
- **Admission Types**: Elective, Emergency, and Urgent care

### Resource Forecasting
- **Predicted Volume**: Steady patient volume for next 6 months
- **Staffing Recommendation**: Current levels sufficient (no major spikes forecasted)
- **Capacity Planning**: Hospital can maintain existing resource allocation

## 🎯 Business Value

1. **Strategic Planning**: Revenue forecasting enables proactive budget planning
2. **Resource Optimization**: Staffing predictions reduce operational costs
3. **Risk Management**: Early identification of high-cost patient segments
4. **Performance Monitoring**: Real-time KPIs for operational efficiency
5. **Data-Driven Decisions**: Evidence-based insights for healthcare administrators

## 📊 Dashboard Features

### Interactive Elements
- Dynamic slicers for multi-dimensional analysis
- Drill-through capabilities for detailed exploration
- Cross-filtering across all visualizations
- Custom tooltips with contextual information

### Visual Components
- **Cards**: Key performance indicators
- **Line Charts**: Trend analysis over time
- **Bar Charts**: Comparative analysis
- **Tables**: Detailed data breakdowns
- **Stacked Charts**: Composition analysis

## 🚀 Getting Started

### Prerequisites
- Power BI Desktop (latest version)
- Windows 10 or later / macOS with Power BI app

### Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/healthcare-analytics-dashboard.git
cd healthcare-analytics-dashboard
```

2. Open the Power BI file:
   - Navigate to `dashboards/helthcare_dashboard.pbix`
   - Open with Power BI Desktop

3. Load the data:
   - The dashboard is pre-configured with the cleaned dataset
   - Data source: `data/healthcare_dataset_cleaned.csv`

### Usage

1. **Refresh Data**: Click "Refresh" in Power BI to load latest data
2. **Interact with Filters**: Use slicers to filter by medical condition, gender, age group, etc.
3. **Explore Dashboards**: Switch between operational overview and strategic forecasting views
4. **Export Reports**: Generate PDF or PowerPoint exports for presentations

## 📋 Dataset Information

### Source Data Fields
- **Patient Information**: Name, Age, Gender, Blood Type
- **Medical Details**: Medical Condition, Doctor, Hospital, Medication
- **Admission Data**: Date of Admission, Discharge Date, Admission Type, Room Number
- **Financial Data**: Billing Amount, Insurance Provider
- **Clinical Results**: Test Results (Normal/Abnormal/Inconclusive)
- **Metrics**: Length of Stay (Days)

### Data Volume
- **Total Records**: 54,966 patient admissions
- **Time Period**: 2019-2024 (with forecasts through 2026)
- **Medical Conditions**: 6 primary conditions tracked
- **Insurance Providers**: 5 major providers (Cigna, Medicare, UnitedHealth, Blue Cross, Aetna)

## 🔍 Analysis Methodology

### Time Series Forecasting
- Historical trend analysis (2019-2024)
- Exponential smoothing for revenue predictions
- Confidence intervals for uncertainty quantification
- Seasonal decomposition for pattern identification

### Statistical Analysis
- Descriptive statistics for KPIs
- Comparative analysis across patient segments
- Cost distribution analysis by medical condition
- Average calculations with outlier handling

### Business Intelligence
- Year-over-year growth analysis
- Provider performance benchmarking
- Resource utilization metrics
- Risk scoring for high-cost patients

## 🎨 Design Principles

- **User-Centric**: Intuitive navigation and clear visual hierarchy
- **Responsive**: Adapts to different screen sizes and devices
- **Accessible**: Color-blind friendly palettes and clear labeling
- **Professional**: Clean, modern aesthetic suitable for executive presentations
- **Interactive**: Dynamic filtering for ad-hoc analysis

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 Future Enhancements

- [ ] Real-time data integration via APIs
- [ ] Predictive modeling for patient readmission risk
- [ ] Advanced machine learning for cost optimization
- [ ] Mobile app version of key dashboards
- [ ] Integration with electronic health records (EHR) systems
- [ ] Automated alert system for anomaly detection
- [ ] Natural language query interface

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Your Name**
- GitHub: [@yourusername](https://github.com/yourusername)
- LinkedIn: [Your LinkedIn](https://linkedin.com/in/yourprofile)
- Email: vaibhavvermaaa123@gmail.com

## 🙏 Acknowledgments

- Healthcare data analytics community for best practices
- Power BI community for visualization inspiration
- Healthcare providers for domain expertise
- Open source contributors

## 📸 Screenshots

### Dashboard 1: Healthcare Operational Performance Overview
![Operational Performance](screenshots/healthcare_operational_overview.png)

*Comprehensive view of operational metrics including admissions, billing, and patient demographics*

### Dashboard 2: Strategic Revenue Forecasting & Risk Analysis
![Revenue Forecasting](screenshots/strategic_revenue_forecasting.png)

*Strategic insights with revenue forecasting, clinical trends, and resource planning*

---

**⭐ If you find this project helpful, please consider giving it a star!**

**📧 Questions or Feedback?** Feel free to open an issue or reach out directly.

---

*Last Updated: February 2026*

