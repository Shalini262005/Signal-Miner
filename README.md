# SignalMiner – Real-Time Growth Signal Tracker from LinkedIn Job Posts

## Project Overview

Startups leave behind digital footprints as they grow — especially through job postings. From hiring product leaders to building global sales teams, LinkedIn job listings reveal high-signal business moves.

SignalMiner is a data-driven analysis project aimed at mining these growth indicators from the hiring activity of Indian startups. It scrapes, cleans, and tags job listings with strategic business signals, helping investors, founders, and recruiters identify momentum before it hits the news.


## Objective

To design a system that detects early signs of startup growth by analyzing structured hiring data from public LinkedIn job listings.


## What This Project Does

- Scrapes job postings of 10–15 Indian startups using Google-powered LinkedIn queries

- Extracts structured fields: company, job title, department, location, seniority, and job URL

- Cleans and standardizes the scraped data for consistency

- Applies rule-based tagging to assign growth signals like “GTM Expansion” or “Talent Funnel”

- Summarizes key insights into hiring trends and business strategies

- Presents the final dataset in CSV format and a polished summary report


## Tools & Technologies Used

| Task               | Tools Used                              |
| ------------------ | --------------------------------------- |
| Web Scraping       | `requests`, `BeautifulSoup`, `Selenium` |
| Data Cleaning      | `pandas`, `regex`, Jupyter Notebook     |
| Tagging Logic | Custom rule-based functions                |
| Reporting          | Notion                         |


## Repository Structure

```
.
├── Scraped_raw_data/
│   ├── Data_scraping.ipynb              - Jupyter notebook for scraping logic
│   └── raw_data.csv                     - Unprocessed scraped job data
│
├── Cleaned_data_with_tags/
│   ├── Data_cleaning.ipynb              - Data transformation, cleaning, and tagging logic
│   ├── Cleaned_data.csv                 - Cleaned dataset (without tags)
│   └── overall_growth_tags.csv          - Final dataset with growth signal tags
│
└── README.md                            - Project documentation
```

## Dataset Fields

| Column Name         | Description                                  |
| ------------------- | -------------------------------------------- |
| company\_name       | Name of the startup                          |
| job\_title          | Job title as listed on LinkedIn              |
| department          | Functional area (e.g., Sales, Product)       |
| location            | Hiring location or remote                    |
| seniority           | Level (Intern, Junior, Mid, Senior, CXO)     |
| url                 | Direct link to job posting                   |
| growth\_signal\_tag | Strategic signal inferred from role patterns |


## Growth Signal Tags – Examples

- GTM Expansion – Multiple Sales/BD/Marketing roles

- New Product Initiative – Product + Design + PM hiring

- Talent Funnel – Hiring 3+ interns across functions

- International Push – Remote roles in global regions

- Brand Buildout – Focused hiring in design/content/video


## Insights Summary

- Urban Company shows a sharp GTM Push with all 26 roles in Business Development, primarily senior-level, across major Indian cities.

- Razorpay is investing in Tech Modernization and Regulatory Focus, with tech and compliance roles (e.g., DevOps, Security, Compliance Engineers).

- Paytm demonstrates a Balanced Growth Strategy through hiring in Sales, Operations, and IT Security — indicating multifaceted expansion.

- Meesho leans into Mid-level Hiring across operational roles, reflecting a Hiring Spree for scaling backend functions.

- Drip Capital and Razorpay highlight Regulatory Compliance as a key hiring area, especially in Risk, Legal, and Analytics roles.

- CRED is hiring cautiously with only 4 open roles in tech and general functions — suggesting a Steady-State or niche approach.

- Senior-level roles dominate leadership hiring across most startups, with Urban Company and Drip Capital leading.

- Geographic Expansion is visible in international roles at Razorpay (Malaysia/Singapore) and Yellow.ai (Indonesia/Remote).

- Zolve and Paytm are focusing on UX/UI revamps, hiring designers and PMs under Product Launch or Design Overhaul tags.

- Internships & Junior Roles in companies like Drip Capital and Groww serve as Talent Pipelines for future scaling.


## Final Deliverables

- Cleaned, tagged dataset (cleaned data with tags.csv)

- Insight report (Notion page)

- Raw scraping and transformation notebooks

- Business signal tagging logic

- Growth insights and startup summaries



## Who This Is For

- VC Analysts scouting early-stage momentum

- Recruiters targeting high-growth tech startups

- SaaS Vendors identifying sales prospects

- Founders benchmarking peer hiring patterns

## Notion Link: 
https://agate-chili-3af.notion.site/Signal-Miner-212cef37d3f880b3ba07cdf73b9744e0?pvs=143
