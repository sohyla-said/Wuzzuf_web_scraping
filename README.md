# Wuzzuf Engineering Jobs Scraper

## 📌 Project Overview
This project is a **Python web scraper** that extracts **engineering job listings** from [Wuzzuf](https://wuzzuf.net) (a major job portal in the Middle East).  
The scraper collects detailed job information and stores it in a structured format (CSV/JSON) for further analysis.  

This tool is useful for **job seekers** and **recruiters** to analyze the engineering job market and discover trends.

---

## ✅ Features
- Extracts key job details:
  - Job Title  
  - Company Name  
  - Job Location  
  - Required Experience Level  
  - Job Posting Date  
  - Required Skills/Qualifications  
  - Job Type (Full-time, Part-time, etc.)  
  - Application Link  

- Handles **pagination** to scrape multiple job listings   
- Implements **respectful scraping** with delays between requests  
- Supports **dynamic content** rendering (via Selenium if required)  
- Cleans and standardizes extracted data  
- Saves results in **CSV/JSON** format  

---

## 🛠️ Technical Requirements
- **Python 3.x**
- Libraries used:
  - `Selenium` (for dynamic content rendering)
  - `csv`, `json` (for saving structured data as CSV/JSON)
  - `time` (for request delays)
- WebDriver (e.g., ChromeDriver)

---

## 🚀 How It Works
1. Opens Wuzzuf job search page with the desired engineering keyword.  
2. Extracts job listings from each results page.  
3. Navigates through pagination until no more results are found.  
4. Extracts job details and required skills.  
5. Cleans and formats the extracted data.  
6. Saves the results in **CSV/JSON** for further analysis.  

---

## 📂 Output Format
The output file (CSV/JSON) contains structured job data like:

```json
{
    "Job Id": 1,
    "Job Title": "Senior Facilities Engineer",
    "Company Name": "Confidential -",
    "Location": "New Capital, Cairo, Egypt",
    "Experience Level": "Experienced",
    "Years of Experience": " 5 - 7 Yrs of Exp",
    "Posting Date": "10 days ago",
    "Required Skills": [
      "Facilities Engineering",
      "Facility Management"
    ],
    "Job Type": "Full Time",
    "Application Link": "https://wuzzuf.net/jobs/p/ipnk1fkfvybq-senior-facilities-engineer-midar-for-investment-and-urban-development-cairo-egypt"
  }

