# Shopify-App-Analysis-Project

## Deployment Instructions
Deployment: The Power BI project requires deployment to a cloud-based service such as Power BI Service or an on-premises Power BI Report Server for sharing and collaboration.

System Requirements: The project necessitates the latest version of Power BI Desktop for report authoring and development, along with compatible versions of Microsoft Office for data source integration. Additionally, ensuring the availability of appropriate data connectors and plugins for databases or applications used in the project is essential for seamless functionality.

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
   ![image](https://github.com/user-attachments/assets/0708ef61-94d9-4f35-ac29-f350788aba6c)

* Line Chart: Review Count vs Lastmod Date
  * Sum of the review count on the Y-axis vs the lastmod date on the X-axis.
  ![image](https://github.com/user-attachments/assets/e9bb0d17-e7c4-40a6-ae59-5ea5685c958e)

* Scatterplot: Reviews Count vs Average Rating
  * Reviews count on the X axis and the average rating on the Y axis with interpretation in a text box.
  ![image](https://github.com/user-attachments/assets/3aeff73b-a09f-48e3-839a-1a7a6e99cafd)

  
### Part 2: Reviews
* Reviews Sheet
  * New sheet in the Power BI file for analyzing reviews.
* KPI Card: Average Value of Helpful Reviews
  * Average value of the new helpful_reviews column.
   ![image](https://github.com/user-attachments/assets/06ccb77a-6a38-49ca-b459-c409b6ecf153)

* Scatterplot: Average Rating vs Developer Answered
  * Comparison of the average rating on the Y-Axis by the value of the developer_answered column on the X-Axis.
  ![image](https://github.com/user-attachments/assets/794f361e-448d-4d02-b278-60e20e024c01)


  * False or if the developer did not answer, there's an average rating of 4.78, while True, or if the developer did answer, we have an average rating of 4.48. So apps where the developer answered show lower average ratings scores then apps where the developer did not answer.

### Part 3: App Reviews
* App Reviews Sheet
  * New sheet in the Power BI file for analyzing app reviews.
* Bar Chart: Sum of Rating by Developer
  * Developer on the X-Axis and the sum of rating on the Y-Axis.
  ![image](https://github.com/user-attachments/assets/f06d141d-7a60-4022-a827-22fa5aeb771a)

* Bar Chart: Helpful Review Average by Developer
  * Developer on the X-Axis against the helpful_review average on the Y-Axis.
  ![image](https://github.com/user-attachments/assets/2533d426-b4bb-42d8-a97f-9fc555936635)

* Bar Chart: Most Responsive Developers
  * Developer from the apps table and the developer_answered column with a filter for rows where reviews_count is greater than 500.
 ![image](https://github.com/user-attachments/assets/59347fa6-6de4-4c53-a396-e9d39c01d740)

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
