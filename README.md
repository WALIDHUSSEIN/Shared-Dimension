Power BI Project:

Creating Shared Dimensions from Fact Tables

Overview
This project demonstrates how to create a star schema data model in Power BI by deriving shared dimension tables from multiple fact tables using Power Query. The goal is to transform a flat data structure into a more optimized relational model by ensuring one-to-many relationships between dimension and fact tables, improving data organization and reporting performance.

Key Concepts

Star Schema:
A simplified relational data structure consisting of a central fact table surrounded by dimension tables, allowing for efficient querying and reporting.

Fact Tables:
Tables that contain transactional or measurable data, such as sales, products, or orders.

Dimension Tables:
Tables that contain descriptive attributes related to the facts, such as product details, store locations, or dates.

One-to-Many Relationship:
A relationship where each record in the dimension table can relate to multiple records in the fact table, but each fact record links to a single dimension record.
Features
Extract shared dimensions such as Date, Product, and Store from fact tables using Power Query.
Automatically generate custom dimension tables using Power Query functions.
Transform raw data into a star schema model, improving filter context flow and report performance.
Ensure filter propagation from dimension tables to fact tables in Power BI for effective data slicing and dicing.
Steps

Import Fact Tables:
Load your fact tables into Power BI from your data sources.

Create Shared Dimensions:

Use Power Query to extract unique lists of values from fact tables for each dimension (e.g., products, dates, stores).
Transform these lists into separate dimension tables.
Optionally, use a custom date table by generating a table with Power Query functions.

Model the Data:

Create a one-to-many relationship between each dimension table and the relevant fact table.
Ensure that dimension tables sit on the "one" side of the relationship, while fact tables sit on the "many" side.

Validate Relationships:

Test the filter context propagation to verify that the model is functioning correctly.
Build Reports: Utilize the star schema model to build efficient and insightful reports, using dimensions for filtering and grouping data.

Pro Tips

When creating the date dimension, leverage Power Query to automatically generate a date table based on the minimum and maximum dates from the fact tables. Use the column profiling feature to quickly identify these values.
Keep your data model clean by avoiding many-to-many relationships, which can lead to performance issues and ambiguous filtering.

How to Use

Clone or download this repository.

Open Power BI and import the Power BI file (.pbix).
Load your own datasets or use the provided sample data to explore the shared dimension creation process.
Follow the Power Query scripts and steps outlined in this project to build your own star schema model.
