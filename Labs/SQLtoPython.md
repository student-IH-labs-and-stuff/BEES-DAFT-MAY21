![Ironhack logo](https://i.imgur.com/1QgrNNw.png)

# Lab | End to End : SQL query & Data Cleaning/Wrangling in Python & Visualise in Python or Tableau

## Introduction

We keep seeing a common phrase that 80% of the work of a data scientist is data cleaning. We have no idea whether this number is accurate but anyone working with data certainly spends lots of time and effort in collecting, cleaning and preparing the data ready for analysis. This is because datasets are usually messy and complex in nature. It is a very important skill to be able to refine and restructure datasets into a usable state in order to proceed to the data analysis stage.

In this exercise, you will both practice the data cleaning techniques, SQL querying we discussed in the lessons this week and apply the new technique of joining python with sql. You will work on your own but remember the teaching staff are at your service whenever you encounter problems.

## Getting Started


In this lab you will be working on [sqlpy-sakila_or_bank.ipynb](sqlpy-sakila_or_bank.ipynb). Download the jupyter file to get started. 

When you are on `sqlpy-sakila_or_bank.ipynb`, read the instructions for each part of the process and provide your answers with the correct code. Make sure to test your answers in each cell and save the notebook. Jupyter Notebook should automatically save your work progress. But it's a good idea to periodically save your work manually just in case.

## Goals

In this lab, you will be retrieving data from your mysql server, either on the sakila or bank databases which you are very familiar with, in order to visualise some business insight (answer a data question in a visual way)


You will need to import the `pymysql` library and the `create_engine` function from the `sqlalchemy` library to connect python and MySQL as you saw in class today.

```python
import pymysql
from sqlalchemy import create_engine
```

Once your connection is established with the database you will use some basic SELECT queries to retrieve the data you want in order to answer the questions.

:bulb: If you receive import errors for `pymysql` or `sqlalchemy`, it means you need to install them with `conda install` or `pip install`.

:bulb: you can also go through [this blog](https://hackersandslackers.com/pandas-and-sqlalchemy/) step by step to complete your installation 

### Challenge Steps

1. Install the required software to connect python and MySQL (see above) 
2. Connect to the server and collect all the appropriate data from users and posts tables with the support of MySQL queries.
3. Create a dataframe from your query.
5. Change the data types of your merged dataset as needed
6. Export the merged data set to csv - potentially filtered to a subset of rows by date or a subset of useful columns. 
7. Summarise and visualise your insight in the data. You can visualise this inside Python using one of the visualisation libraries (seaborn/matplotlib/bokeh/plotly), or if you prefer, by connecting to the csv with Tableau.
8.  Bonus - add in other interesting features to your visualisations. 
9.  publish the csv, your completed jupyter notebook and any visualisations to a github repo and submit the url to github via the student portal (if you are using Tableau, save the workbook to your tableau public account and publish the url on your github readme)


### What do we really want to know from the data ? 

:bulb: if you are struggling with SQL and Python today, but you still want to do some nice visualisations during this lab, here is an option for you. I have uploaded an excel file containing data about the [top 500 youtube gamers](500_YouTube_Games.xlsx) (warning : out of date, from 2017) which you can read into python or directly visualise in tableau.  In this case you will be looking at the relationship between youtube accounts, subscribers and views and can still do some interesting data analysis and insight. 


**:exclamation: If you feel you are already good at Python/Pandas and don't need the instructions in `sqlpy.ipynb` to walk you through the steps, please feel free to skip `sqlpy-sakila_or_bank.ipynb` and create your own solution files.**

## Deliverables

- `sqlpy-sakila_or_bank.ipynb` with your completed code.
- `data.csv` containing the 'cleaned' dataset.
- visualisation inside `sqlpy-sakila_or_bank.ipynb` or other tool, such as tableau public url or a published workbook/excel chart exported as png.  

## Submission

Upon completion, add your deliverables to git, commit your code and submit to your github repo, which would likely include running the below from your command line

  ```
  git add .
  git commit -m "<lab or project name>"
  git push origin master
  ```
Do ensure you have a tidy, readable .md file for your lab.

- you can then submit your github url via the Student Portal

## Refresher resources on data cleaning if needed 

[Data Cleaning with Numpy and Pandas](https://realpython.com/python-data-cleaning-numpy-pandas/#python-data-cleaning-recap-and-resources)

[Data Preparation](https://www.kdnuggets.com/2017/06/7-steps-mastering-data-preparation-python.html)

[Google Search](https://www.google.es/search?q=how+to+clean+data+with+python)
