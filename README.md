# Dashboards
**About**

Welcome to my little collection of Tableau and Power BI dashboards and reports. 

# Project 1: Tracking program KPIs in Power BI

This project was focused on tracking KPIs for multiple teams who complete a program renewal process each year for their clients. They wanted to track what statuses client renewals were in, including how many had been completed. They also wanted to filter based on client regions. I used DAX studio to add a visual showing which filters were applied. 

**Data used**

Most of the data here was extracted daily from an excel file and stored in a SharePoint list that was being modified as team members processed client renewals. I also added to the model an Oracle table holding specific region information and joined it to existing data using a unique client identifier. In this case, we also wanted to be able to filter by all regions (of Texas) and local health departments. To do this, I created a hierarchy of regions and local health departments within each to allow users to select specific areas.

![renewal_dashboard](https://github.com/user-attachments/assets/9e789011-db92-42ca-be02-115ca0cfc804)


# Project 2: Data quality in Tableau

This report was requested for staff to track the increase of a specific data point (clients) that were being duplicated in their database due to errors in the data ingested. They wanted to see how fast the duplicates were growing, how quickly they were being removed (merged), and which teams were removing them (this has been blocked out for privacy). This team did not want any filters in the report as they wanted a static file.

**Data used**

The tables needed for this report were quite large, with some over 2 million rows. I opted for transforming and joining the data in Tableau and caching an extract which refreshed weekly. Six database tables were joined to get all the counts needed. Also appended to the removed/merged client count was an excel file with recently manually reviewed duplicate client accounts that were not reflected in the database.

<img width="612" alt="Example_merges" src="https://github.com/user-attachments/assets/54ce5609-5a9d-4bc5-8f94-56681ea0e70b">


