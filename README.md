# Shopify-App-Analysis-Project

## Deployment Instructions
Deployment: The Power BI project requires deployment to a cloud-based service such as Power BI Service or an on-premises Power BI Report Server for sharing and collaboration.

System Requirements: The project necessitates the latest version of Power BI Desktop for report authoring and development, along with compatible versions of Microsoft Office for data source integration. Additionally, ensuring the availability of appropriate data connectors and plugins for databases or applications used in the project is essential for seamless functionality.

## Demo Video
https://www.loom.com/share/5da606ebe68e499083b4980a31af0503?sid=9ad2df3f-3f12-4b06-8fef-3d9abf68115e

## Table of Contents

### Introduction
### The Data
### Part 1: App Landscape
* App Landscape Sheet
* KPI Card: Unique Number of Apps
* Line Chart: Review Count vs Lastmod Date
* Scatterplot: Reviews Count vs Average Rating
### Part 2: Reviews
* Reviews Sheet
* KPI Card: Average Value of Helpful Reviews
* Scatterplot: Average Rating vs Developer Answered
### Part 3: App Reviews
* App Reviews Sheet
* Bar Chart: Sum of Rating by Developer
* Bar Chart: Helpful Review Average by Developer
* Bar Chart: Most Responsive Developers

### Part 4: Conclusions
----------------------------------
### Introduction
* You have been hired to review the landscape of apps on the Shopify platform, using data scraped from publicly available Shopify websites. This project aims to figure out the key factors that contribute to the success of a Shopify app.

### The Data
* The shopify.xlsx dataset contains public data scraped from the Shopify App Store. It includes four tables:
  * apps: Details of the apps on Shopify apps marketplace.
  * apps_categories: Join tables to connect apps with categories.
  * categories: Categories of the apps. Each app has multiple categories.
  * reviews: Each review (row) contains information on user opinion about the related app (rating and comment). Also, it contains the response from the developer if present.
    
### Part 1: App Landscape
* App Landscape Sheet
  * New sheet in Power BI (.pibx) file for analyzing app landscape.
* KPI Card: Unique Number of Apps
  * Counts the unique number of apps.
   <img width="476" alt="Screen Shot 2024-02-20 at 4 48 24 PM" src="https://github.com/Robblodo11/Airbnb-Rental-Marker-Analysis-READ.ME/assets/153016872/e988ec59-db65-406a-919f-4f42ab68a95a">
* Line Chart: Review Count vs Lastmod Date
  * Sum of the review count on the Y-axis vs the lastmod date on the X-axis.
  <img width="568" alt="Screen Shot 2024-02-20 at 4 49 37 PM" src="https://github.com/Robblodo11/Airbnb-Rental-Marker-Analysis-READ.ME/assets/153016872/d5d831d4-cc59-43f0-82de-b0c107068f78">
* Scatterplot: Reviews Count vs Average Rating
  * Reviews count on the X axis and the average rating on the Y axis with interpretation in a text box.
  <img width="567" alt="Screen Shot 2024-02-20 at 4 50 26 PM" src="https://github.com/Robblodo11/Airbnb-Rental-Marker-Analysis-READ.ME/assets/153016872/81c54c39-97ef-48ec-8039-3d74d91aa28f">
  
### Part 2: Reviews
* Reviews Sheet
  * New sheet in the Power BI file for analyzing reviews.
* KPI Card: Average Value of Helpful Reviews
  * Average value of the new helpful_reviews column.
   <img width="436" alt="Screen Shot 2024-02-20 at 4 51 13 PM" src="https://github.com/Robblodo11/Airbnb-Rental-Marker-Analysis-READ.ME/assets/153016872/dd7b34cc-8314-4787-90bb-110c3c672fc7">
* Scatterplot: Average Rating vs Developer Answered
  * Comparison of the average rating on the Y-Axis by the value of the developer_answered column on the X-Axis.
  <img width="522" alt="Screen Shot 2024-02-20 at 4 51 54 PM" src="https://github.com/Robblodo11/Airbnb-Rental-Marker-Analysis-READ.ME/assets/153016872/5400ce42-0654-4728-a897-e63fd766c727">

  * False or if the developer did not answer, there's an average rating of 4.78, while True, or if the developer did answer, we have an average rating of 4.48. So apps where the developer answered show lower average ratings scores then apps where the developer did not answer.

### Part 3: App Reviews
* App Reviews Sheet
  * New sheet in the Power BI file for analyzing app reviews.
* Bar Chart: Sum of Rating by Developer
  * Developer on the X-Axis and the sum of rating on the Y-Axis.
  <img width="391" alt="Screen Shot 2024-02-20 at 4 53 12 PM" src="https://github.com/Robblodo11/Airbnb-Rental-Marker-Analysis-READ.ME/assets/153016872/e562efbd-69c8-4f50-9631-7e368ed25707">
* Bar Chart: Helpful Review Average by Developer
  * Developer on the X-Axis against the helpful_review average on the Y-Axis.
  <img width="392" alt="Screen Shot 2024-02-20 at 4 54 03 PM" src="https://github.com/Robblodo11/Airbnb-Rental-Marker-Analysis-READ.ME/assets/153016872/69f1c1c7-31a3-46c4-9ce8-c063f5b03897">
* Bar Chart: Most Responsive Developers
  * Developer from the apps table and the developer_answered column with a filter for rows where reviews_count is greater than 500.
  <img width="377" alt="Screen Shot 2024-02-20 at 4 54 46 PM" src="https://github.com/Robblodo11/Airbnb-Rental-Marker-Analysis-READ.ME/assets/153016872/10f3f2fc-3ae9-4ffe-921e-795180d58dc4">

### Part 4: Conclusions
* The total number of unique apps available on the Shopify platform is 7,341.
* There was a significant decline in review counts observed from May 9th to May 10th, followed by fluctuations until June 4th.
* A scatterplot analysis revealed a weak, positive relationship between review counts and average ratings, suggesting that higher review counts do not necessarily equate to higher ratings.
* The creation of a new column called "helpful_reviews" weighted the reviews based on their perceived helpfulness, which allowed for a more nuanced understanding of the reviews' impact.
* A correlation was observed between developer responsiveness and average ratings. Apps where developers answered user reviews tended to have lower average ratings compared to those where developers did not respond.
* Visualizations on the developer's performance indicated:
  * The sum of ratings attributed to each developer.
  * The average of helpful reviews per developer, aiming to mitigate the influence of potential skewed ratings.
  * The responsiveness of developers to user reviews, highlighting which developers are more proactive in engaging with their users.
  * A filter was applied to focus on developers with a significant review count, suggesting a more established presence in the app ecosystem.
* Overall, these insights suggest that success on the Shopify platform is influenced not only by the quantity of reviews and interactions but also by the quality and timeliness of developer responses. Additionally, while higher review counts may contribute to visibility, they do not guarantee higher ratings, emphasizing the importance of user satisfaction and engagement in app success.
