# Tackling the Health Crisis in Africa 

![© Unsplash](https://github.com/Dee-nDee/Tackling-the-Health-Crisis-in-Africa/blob/master/unsplash-health-africa.jpg) 

## Table of Contents 

<ul>    
<li><a 
href="#overview">Project Overview</a></li>     
<li><a 
href="#install and setup">Installation and Setup</a></li> 
<li><a 
href="#codes and resources">Codes and Resources Used</a></li> 
<li><a    
href="#data">Data</a>
    <ul> 
        <li><a href="#source">Source Data</a></li>
        <li><a href="#pre-processing">Data Pre-processing</a></li>         
        </ul>
    </li>     
<li><a 
href="#results">Results</a></li> 
<li><a 
href="#acknowledgement">Acknowledgement</a></li>       
</ul> 


<a id='overview'></a>

# Project Overview  

This project focuses on obtaining insights into the health situation in Africa, which will aid in identifying appropriate solutions to the continent's ongoing health crisis and lower the number of deaths that are reported in Africa each year. 


<a id='install and setup'></a>

# Installation and Setup 

```

import numpy as np 

import pandas as pd 

import matplotlib.pyplot as plt 

import seaborn as sb 

import sqlite3 

sb.set_style("darkgrid")

%matplotlib inline 

!pip install ipython-sql

``` 


<a id='codes and resources'></a>

# Codes and Resources Used   

**Python Version** - Python 3 

- **Data Wrangling** - `pandas`, `numpy`, `sqlite3` 

- **Exploratory Data Analysis** - `sqlite3`

- **Data Visualization** - `seaborn`, `matplotlib`



<a id='data'></a>

# Data

<a id='source'></a>

## Source Data 

Six datasets are used in this analysis. These datasets can be found [here](https://d2ag3jdu89hmr4.cloudfront.net/link_click/Clv2b0DOAo_xkEd5/af3b1c9887c1dae38acd4dfb3d1b19ba). They are stored as: 

- `1. annual-number-of-deaths-by-cause.csv` 

- `2. number-of-deaths-by-age-group.csv` 

- `3. Medical Doctors Per 10000 population.xlsx` 

- `4. ISO 3166_country-and-continent-codes-list-csv.csv` 

- `5. World Population.csv`

- `6. Current health expenditure (% of GDP).xlsx`

The above were renamed: 

- `annual-number-of-deaths-by-cause.csv`

- `number-of-deaths-by-age-group.csv`

- `Medical Doctors Per 10000 population.xlsx`

- `ISO3166_country-and-continent-codes-list-csv.csv`

- `World_Population.csv`

- `Current health expenditure (% of GDP).xlsx` 


<a id='pre-processing'></a>

## Data Pre-processing 

The datasets were cleaned twice, using Python and SQL.

**Data cleaning with Python** <br>
Python was mostly utilized to restructure the tables in order to provide a tidy dataset. Additionally, it was used to modify column names, remove unnecessary columns, and change variable data types as needed.

**Data Cleaning with SQL**<br>
SQL was used to modify the datasets to solely obtain data related to Africa. 

**Database Creation**<br> 
After the preliminary cleaning with Python, the datasets were entered into a database, [Health_Crisis.db](https://drive.google.com/file/d/1wDbuR1R8DhuBN0wT2OC8FmboGrAOyhji/view?usp=drivesdk) to facilitate analysis with SQL. 


<a id='results'></a>

# Results 

In Africa, there is a high mortality rate from cardiovascular diseases, neonatal disorders, HIV/AIDS, lower respiratory infections, and diarrheal diseases, with children under the age of five having the highest mortality rates. 

Additionally, of the 54 countries in Africa, 19 account for a significant portion of the continent's annual mortality, with Nigeria, the continent's most populated nation, taking the top spot by a large margin.  


<a id='acknowledgement'></a>

# Acknowledgement

 - [praggy/datascience-readme-template](https://github.com/pragyy/datascience-readme-template) 
