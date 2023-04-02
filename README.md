# TECA Data Analysis

![](Photo_1679140738060.png)

## Introduction
TECA is acompany that owns over 150 convenience stores and gas stations throughout the middle of the United States. These stores sell typical convenience store items: gas candy, soda, chips, lottery tickets and so on. A sample of 3,000 rows and 23 variables of **TECA's point of sale** data during the years of 2017 - 2019 is used for the analysis. Each row of this dataset represents a unique product of a single transaction.
Columns in this dataset contain information about five main categories of the transaction:
- When items sold
- Customers sold to
- What product sold
- Store location
- Revenue and Profit data

## Questions About Business Insights

1. What is the peak day and month for 2018 summer sales?
2. What is the peak day and month for 2018 winter sales?
3. Which products sold most during both seasons?
4. Which states recorded the highest sale during both seasons?
5. What are complementary products that customers often purchase together so that we can place them next to each other?
6. What are the top 5 most sold products?
7. What are the top 5 high profit margin products?
8. Which stores are performing best?
9. Which stores are selling energy drink at high rate?
9. Which stores are selling fuel at high rate?

## Skills/ Concepts Demonstrated

The following PowerBI features were incorporated:
- Range of attractive visualizations 
- Get data feature 
- Datasets filtration 
- Data Analysis Expressions DAX
- Page navigation
- Modelling
- Tooltips 
- Buttons

## Examining Data With Power Query Editor

![](https://github.com/kemiscut/TECA-Data-Analysis/blob/93082ebd86ce4852fcd2004e57032989132bc46d/column%20profiling.jpg)

Each column was changed to its proper data type. Profiling the revenue column,I checked the Min, Max, Avg and the Standard deviation. The standard deviation is about 26 and if this were a normally distributed column of data, then any outliers are typically either above three standard deviations above the mean or three standard deviation below the mean.
So if I take 26 and multiply by 3, that's about 78 and then add that to the average 8that means anything that's above 86 would be considered an outlier and if I take that 78 and subtract it from , that means anything below -70 would be considered an outlier as well.

Unclean TecaPosSmall Table       |       Cleaned TecaPosSmall Table
:-------------------------------:|:-------------------------------:
![](https://github.com/kemiscut/TECA-Data-Analysis/blob/93082ebd86ce4852fcd2004e57032989132bc46d/data%20cleaning%202.jpg)| ![](https://github.com/kemiscut/TECA-Data-Analysis/blob/93082ebd86ce4852fcd2004e57032989132bc46d/data%20cleaned.jpg)

Unclean State Table              |       Cleaned State Table
:-------------------------------:|:-------------------------------:
![](https://github.com/kemiscut/TECA-Data-Analysis/blob/93082ebd86ce4852fcd2004e57032989132bc46d/state%20uncleaned.jpg)| ![](https://github.com/kemiscut/TECA-Data-Analysis/blob/93082ebd86ce4852fcd2004e57032989132bc46d/state%20cleaned.jpg)

## Data Modelling

Since the datasets consist of two tables, a many to one relationship was automatically generated by PowerBI. The zip column in TecaPosSmall table linked to the postal code column in the States table.

![](https://github.com/kemiscut/TECA-Data-Analysis/blob/93082ebd86ce4852fcd2004e57032989132bc46d/data%20model.jpg)

## Data Visualization

The report comprises 3 pages
- Seasonal sales
- Products
- Stores

![](https://github.com/kemiscut/TECA-Data-Analysis/blob/93082ebd86ce4852fcd2004e57032989132bc46d/teca%202_page-0001.jpg)
![](https://github.com/kemiscut/TECA-Data-Analysis/blob/93082ebd86ce4852fcd2004e57032989132bc46d/teca%202_page-0002.jpg)
![](https://github.com/kemiscut/TECA-Data-Analysis/blob/93082ebd86ce4852fcd2004e57032989132bc46d/teca%202_page-0003.jpg)
You can interact with the report [here]()

