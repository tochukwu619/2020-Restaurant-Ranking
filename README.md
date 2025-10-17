# 2020-Restaurant-Ranking
This is the ranking of restaurants in the US for the year 2020 by the restaurant business magazine.


### Overview

This data was obtained from the rankings by “The Restaurant Business Magazine” in the US for the pandemic period of 2019.  The data can be used to tell the story of what 2020 was like for restaurants, what was hot, what could be more popular soon, or what the difference is between large companies and smaller businesses.


### Data Source

The data is sourced from [Kaggle](https://www.kaggle.com/datasets/michau96/restaurant-business-rankings-2020?resource=download)


### Tools

Microsoft Excel --> [here](www.office.com)


### Data Description

The data is in 3 CSV files, top 250 (250 rows, 9 columns), independence 100 (100 rows, 7 columns), and future 50 (50 rows, 9 columns). 

The features of the top 250 are:

| Feature  |	Description  |
|----------  | ------------  |
| Rank  |	Position in ranking  |
| Restaurant  |	Name of restaurant  |
| Content  |	Description, only for certain restaurants  |
| Sales  |	 ($000000)  |
| YOY_Sales  |	Year on year sales increase in %  |
| Units  |	Number of premises in US  |
| YOY_Units  |	Year on year premises increase in %  |
| Headquarters  |	Place of the restaurant's headquarters  |
| Segment_Category  |	Menu Type  |

The features of the independence 100 are:

| Features  |	Description  |
| --------- | ------------ |
| Rank  |	Position in ranking  |
| Restaurant  |	Name of restaurant  |
| Sales  |	Annual sales in $  |
| Average Check  |	Average client expenses per visit (sales/number of visits)  |
| City  |	City of origin of the restaurant  |
| State  |	State of origin of the restaurant  |
| Meals Served  |	Number of meals served  |

The features of the future 50 are:

| Features  |	Description  |
| --------- | ----------- |
| Rank  |	Position in ranking  |
| Restaurant  |	Name of restaurant  |
| Location  |	Location of origin of the restaurant  |
| Sales  |	Systemwide Sales ($000000)  |
| YOY_Sales  |	Year on year sales increase in %  |
| Units  |	Number of premises  |
| YOY_Units  |	Year on year premises increase in %  |
| Unit_Volume  |	Average Unit Volume ($000)  |
| Franchising  |	Is the restaurant a franchise? (Y/N)  |


### Data Cleaning and Preparation

- From the Independence 100 data, I merged the restaurant, city, and state column, set the correct data type, and changed the abbreviation of the state to fullname using power query in Excel.
- From the Future 50 data, using power query, I split the location column to city and state, and changed the abbreviated state column to the fullname.
- From the Top 250 data, using power query, I removed the content and headquarters columns because they have large percentage of null values.


### Data Analysis

- What are the top 10 states/ menu types represented in the ranking?
  <img width="1653" height="993" alt="Q1 Future" src="https://github.com/user-attachments/assets/4394235c-d795-4296-863a-283c30925116" />

  <img width="1653" height="993" alt="Q1 Independence" src="https://github.com/user-attachments/assets/7425c9f9-c921-484e-b1c9-024411ad8387" />

  <img width="1653" height="993" alt="Q1 Top250" src="https://github.com/user-attachments/assets/f1a578b3-d35e-4083-80ee-0e462c9f0b13" />


- What are the top 5 states/ menu types by average sales?

  <img width="1653" height="993" alt="Q2 future" src="https://github.com/user-attachments/assets/94f8e938-4d08-4a7c-89d0-cadd3d008317" />

  <img width="1653" height="993" alt="Q2 Independence" src="https://github.com/user-attachments/assets/fc724ace-c737-4c46-ab98-4b945bf0661a" />

  <img width="1899" height="993" alt="Q2 Top250" src="https://github.com/user-attachments/assets/3d591917-24b2-45c4-9f39-95029e3b83cf" />


- What are the top 3 restaurants by YOY sales?

  <img width="1653" height="993" alt="Q3 Future" src="https://github.com/user-attachments/assets/77be5148-2fdc-4082-adf4-4ba19c09dde4" />

  <img width="1653" height="993" alt="Q3 Top250" src="https://github.com/user-attachments/assets/b0c81c93-f906-49bc-a651-6e6b101e46bf" />


### Results/ Findings

-	Because there is no correlation by location from the different rankings, location cannot be used as a factor to determine the ranking.
-	More quick services are represented in the ranking and generate the top average sales. We can draw insights that fast food increases sales and ranking.


### Limitations

-	There is no consistency in the features represented from the various rankings.
-	There is a lot of missing data in 2 features from the top 250.
