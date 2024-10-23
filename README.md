# Customers-Chemical-Compliance-Request-Data-Analysis

## Project Overview
This project analyzes customer requests for chemical compliance to improve the management of compliance across various regulations. The aim is to understand processing times, manufacturer response behaviors, and regulation-based requests, which are essential for maintaining compliance and preventing delays in sales.

In the electronics industry, compliance with regulations like ROHS, PFAS, and REACH is vital. Manufacturers must provide documentation, and any delays can lead to penalties or customer dissatisfaction. 

Key analyses include:
- Time taken to process compliance requests.
- Volume of requests for specific regulations.
- Responsiveness of manufacturers.

## Business Problem
The main challenge is understanding service level agreement (SLA) times for chemical compliance requests and identifying suppliers with extensive parts lists. We seek to answer:

- What is the average time to complete a request?
- How many suppliers have numerous parts?
- Which suppliers require company-level documents to speed up completion times?

By analyzing this data, we can identify suppliers that need action to improve request processing, helping the client enhance efficiency in managing compliance requests.

## Dataset Information
- **Request_ID**: Unique identifier for each request.
- **Customer_ship_code**: Code representing the shipping location of the customer.
- **Customer_no**: Unique customer identification number.
- **Customer_name**: Name of the customer.
- **Request_raised_date**: Date when the compliance request was raised.
- **Manufacturer_part_no**: Part number assigned by the manufacturer.
- **Manufacturer_name**: Name of the manufacturer.
- **Manufacturer_code**: Code associated with the manufacturer.
- **Request_Type**: Type of compliance request (e.g., Materials Declaration, ROHS, PFAS).
- **Document_submitted_date**: Date the manufacturer submitted the compliance documentation.
- **Standardized_manufacturer_name**: Cleaned and standardized manufacturer name for uniformity.

## Key Objectives
- **Time Analysis**: Analyze the time taken for manufacturers to submit documents after a compliance request is raised. This will help in identifying bottlenecks.
- **Regulation Insights**: Group compliance requests based on regulation type (e.g., ROHS, PFAS) to understand which regulations are most frequently requested.
- **Manufacturer Performance**: Assess how different manufacturers perform in terms of response time and compliance documentation submission.

## Concepts and Techniques Used
- **Data Cleaning**: Standardized manufacturer names and handled missing or partial data for analysis consistency.
- **Time Series Analysis**: Calculated the day difference between request raised and document submission to assess the responsiveness of manufacturers.
- **Grouping and Aggregation**: Grouped data by manufacturer and request types to identify trends in compliance requests.
- **SQL Queries**: Performed complex queries to extract meaningful insights and compute averages, using MySQL to manage large datasets.

## Key Analysis
- **Day Difference Calculation**: Time taken between the request raised and document submission for each line item, which was then averaged by request ID.
- **Request Type Grouping**: Grouping requests by regulation type and manufacturer to identify high-volume compliance types.
- **Manufacturer Responsiveness**: Analyzed the performance of manufacturers based on their compliance document submission times.

## Conclusion
This project provides valuable insights into the chemical compliance process, helping companies manage compliance more effectively by identifying trends in processing times, compliance types, and manufacturer responsiveness. This analysis can improve compliance tracking, enhance supplier performance, and ensure smooth business operations without delays in product sales.
