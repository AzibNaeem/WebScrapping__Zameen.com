# 🏠 Zameen.com Property Data Scraper & Analysis  
A comprehensive Python-based web scraping and data analysis project that extracts real estate property listings from **Zameen.com** and performs insightful data analysis on **Lahore's housing market**.  

## 📊 Project Overview  
This project automates the collection of property data from **Zameen.com**, Pakistan's leading real estate platform. It scrapes detailed property information across multiple pages, cleans and processes the data, and provides valuable insights into **Lahore's real estate market trends**.  

## 🚀 Features  
- **🔍 Web Scraping**: Automated extraction of property data from Zameen.com  
- **🧹 Data Cleaning**: Comprehensive data preprocessing and normalization  
- **📈 Data Analysis**: Statistical analysis and visualization of property trends  
- **💾 Data Export**: Save results in CSV format for further analysis  
- **🛡️ Error Handling**: Robust error handling and logging  

## 🛠️ Technologies Used  
- **Python 3**  
- **BeautifulSoup4** – Web scraping  
- **Pandas** – Data manipulation and analysis  
- **Requests** – HTTP requests  
- **Regular Expressions** – Data parsing and cleaning  
- **Jupyter Notebook** – Interactive development environment  

## 📁 Project Structure  
📦 Zameen-Property-Scraper  
├── 📄 L23-2541__Assignment_01.ipynb # Main Jupyter notebook  
├── 📊 zameen.csv # Raw scraped data  
├── 📊 zameen_clean.csv # Cleaned and processed data  
└── 📋 README.md # Project documentation  

## 🎯 Data Collection  
### Scraped Data Points:  
- **🏷️ Property Title** – Detailed property description  
- **💰 Price Information**  
  - Original price text  
  - Converted numeric price (PKR)  
- **📍 Location** – Property area and neighborhood  
- **🛏️ Bedrooms** – Number of bedrooms  
- **🚿 Bathrooms** – Number of bathrooms  
- **📏 Area Details**  
  - Original area size  
  - Area unit (Marla/Kanal/Sqft)  
  - Converted square footage  

### Data Processing Features:  
- **Price Conversion**: Handles Pakistani currency formats (Crore, Lakh, Arab)  
- **Area Standardization**: Converts Marla/Kanal to square feet  
- **Duplicate Removal**: Eliminates duplicate entries  
- **Data Validation**: Removes incomplete records  

## 📈 Key Insights  
### Price Analysis:  
- **Right-skewed distribution** indicating most properties are moderately priced  
- **Few extremely expensive properties** creating long tail  
- **Comprehensive price range** from affordable to luxury segments  

### Area Analysis:  
- **Majority mid-sized properties** dominate the market  
- **Very large plots are rare** in the dataset  
- **Consistent unit conversion** for accurate comparisons  

Usage

Open the Jupyter notebook: L23-2541__Assignment_01.ipynb

Run the scraping cells to collect data

Execute data cleaning and analysis cells

Export results to CSV files

📊 Sample Output

The project generates two main output files:

zameen.csv – Raw scraped data with all original fields

zameen_clean.csv – Processed data with:

Standardized price values

Normalized area measurements

Removed duplicates and null values

🔧 Technical Details
Web Scraping Strategy:

Pagination Handling: Scrapes 100 pages with 25 listings each

Rate Limiting: 2-second delays between requests

Error Resilience: Continues scraping even if individual pages fail

User-Agent Rotation: Mimics real browser requests

Data Cleaning Pipeline:

Price Fixing: Converts textual prices to numeric values

Area Conversion: Standardizes area measurements to square feet

Duplicate Removal: Based on title and location combination

Null Value Handling: Removes records with missing essential data

📈 Analysis Capabilities
Current Analysis:

Price distribution trends

Area size patterns

Basic statistical summaries

Potential Extensions:

Location-based price analysis

Price per square foot calculations

Time-series trend analysis

Comparative market analysis

⚠️ Important Notes

Ethical Scraping: Respects website terms of service with reasonable request rates

Data Accuracy: Dependent on source website data quality

Market Changes: Real estate data is time-sensitive and subject to change

🎓 Educational Value

This project demonstrates:

Web scraping best practices

Data cleaning and preprocessing

Real-world data analysis

Pakistani real estate market understanding

Python data science workflow

🤝 Contributing

Feel free to fork this project and submit pull requests for:

Additional data analysis

Improved scraping techniques

Enhanced visualization

New feature implementations

📄 License

This project is for educational purposes. Please ensure compliance with Zameen.com's terms of service when using this code.
