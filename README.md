# Descriptive and Predictive Analytics for Sold eBay Uniqlo Shirts 

In this project, the focus areas were as follows:
* Web scraping eBay's search results page
* Investigating unique characteristics of sold KAWS shirts on eBay with respect to those from other Uniqlo lines
* Constructing a robust price prediction model for sold Uniqlo shirts 

There were 5 major components to this project (outlined below):

## 1) Web Scraping
First, data was scraped from eBay's website. The scraper used in the notebook extracts various information contained in the overall results page when "uniqlo shirt" is entered into a search on sold listings ordered from most recent to least recent and the individual listings pages. The number of results pages to extract is determined by the num_pages variable in the first code cell. Rudimentary stages of data cleaning were performed as well. The output is a csv file. As the section involved building a prototype for executing this process, object oriented programming techniques and concepts can be incorporated to refine this code. 

Code is in `uniqlo_1_scraping.ipynb`.



## 2) Data Wrangling
Then, numerous procedures involving data cleaning, variable addition, and missing transaction time approximation for the scraped data was executed. After these were executed, the final data was filtered to only be shirts sold between the months of May and July: this was then outputted as an Excel file.

Code is in `uniqlo_2_wrangling.ipynb`.


## 3) Dashboard Creation
During the summer of 2019, the KAWS shirt line was a hit: the sold out stores made numerous articles with sensational headlines on the web. This dashboard captures trends and characteristics of sold listings with a focus on relative comparison between KAWS vs. non-KAWS shirts. 

Description is in `uniqlo_3_dashboard.md`. **Dashboard is found at the link below: https://public.tableau.com/profile/edward.shiang#!/vizhome/UniqloKAWSeBayDashboardDemo/KawsDash**

## 4) Data Exploration (WIP)
Here, certain features of the data were investigated through constructing various summary tables and graphs. These insights were then incorporated in the regression models constructed in the following section. 

Code and findings are in `uniqlo_4_eda.ipynb`.

## 5) Predictive Analytics (WIP)
Finally, various regression models for predicting an order price given specific characteristics of the sold listing were constructed, tuned, and relatively compared. Then, additional findings were presented after selecting a specific model from the candidates and leveraging its interpretablility capabilities.

Code and findings are in `uniqlo_5_model.ipynb`.
