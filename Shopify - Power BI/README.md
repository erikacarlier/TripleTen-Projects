## Objective
The objective of this project was to use the data from publicly available Shopify websites to demonstrate which factors contribute to the success of certain shops over others.

## Overview
## Review App Landscape
Find key statistics on the types of apps that are out there. This question uses the Apps table. Make a new sheet in your Power BI (.pibx ) file called App Landscape for this question.
  1. Make a KPI Card (a visual with a single number) that counts the unique number of apps. Add it to your App Landscape sheet.
  2. Make a Line Chart getting the sum of the review count on the Y-axis, and the lastmod date on the X-Axis.
  3. Make a Scatterplot with the reviews_count on the X axis and the average rating on the Y axis. Annotate your interpretation of this with an inserted Text Box next to this scatterplot.

## Reviews
Make a new sheet in your .pibx file for this new section, named Reviews.
  1. Create a new Column in the Reviews table named helpful_reviews using a DAX expression, which multiplies the rating by 1+helpful_count to weigh the reviews by how helpful they’ve been found. The formula in mathematical form would be rating * (1+helpful_count). Make a Card with the average value of the new helpful_reviews column.
  2. Create a new Column in the Reviews table named developer_answered using a DAX expression, which is 1 (or TRUE) if the developer_reply column is not blank and 0 (or FALSE) if the column row is blank. Make a scatterplot comparing the average rating on the Y-Axis by the value of the developer_answered column on the X-Axis.

## App Reviews
Make a new sheet in your .pibx file for this new section, named App Reviews.
  1. In the data model, create a new relationship between the Reviews table and the Apps table. Use the app_id column from the Reviews table, the id column from the Apps table. Make the relationship many-to-one built as many (Reviews table) to one (Apps table). Using this new table, make a bar chart with the developer on the X-Axis, and the sum of rating on the Y-Axis.
  2. The chart in the previous question is misleading because an app could have a high sum of rating because it has many one-star reviews. Make a new bar chart with developer on the X-Axis against the helpful_review average on the Y-Axis.
  3. Which developers are the most responsive? Make a bar chart with the developer from the apps table and the developer_answered column you created in question 2.2. Add a Filter for this visual only which selects only the rows where reviews_count is greater than 500.

## Project Preview
![Sample Image](https://github.com/erikacarlier/TripleTen-Projects/blob/33f8b3f48e942ed458fcbdb23d6f4f4e2979e04f/Shopify%20-%20Power%20BI/Photos/PowerBI_Project_1.2.png)

![Sample Image](https://github.com/erikacarlier/TripleTen-Projects/blob/33f8b3f48e942ed458fcbdb23d6f4f4e2979e04f/Shopify%20-%20Power%20BI/Photos/PowerBI_Project_1.3.png)

![Sample Image](https://github.com/erikacarlier/TripleTen-Projects/blob/33f8b3f48e942ed458fcbdb23d6f4f4e2979e04f/Shopify%20-%20Power%20BI/Photos/PowerBI_Project_3.3.png)
