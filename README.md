# Data-visualization-and-analyzation-using-Python
# Introduction.
Every suicide is a tragedy. According to estimates from the World Health Organization (WHO), over 800,000 people die due to suicide every year. This corresponds to an age-standardized suicide rate of around 11.5 per 100,000 people. This is equivalent to someone dying of suicide every 40 seconds. Yet suicides are preventable with timely, evidence-based interventions.
The mortality data from the WHO suggest that the prevalence and characteristics of suicidal behavior vary widely between different communities, in different demographic groups and over time. One important source of heterogeneity, both globally and within countries, is gender: suicide rates are much higher for males, particularly in high-income countries.
Suicide is an extremely complex issue, and while it is not possible to pin down its causes, there are some risk factors that have been identified, mainly through correlations. Mental health, specifically depression, is widely recognized as the most important risk factor. Here I discuss evidence of this and other important correlates that shed light on possible interventions to prevent suicide.

# Domain Specification.
The dataset has 27.8k entries with 12 attributes. This compiled dataset pulled from four other datasets linked by time and place, and was built to find signals correlated to increased suicide rates among different cohorts globally, across the socio-economic spectrum. Following web sites are the references for that dataset.
• United Nations Development Program. (2018). Human development index (HDI). Retrieved from http://hdr.undp.org/en/indicators/137506
• World Bank. (2018). World development indicators: GDP (current US$) by country:1985 to 2016. Retrieved from http://databank.worldbank.org/data/source/world-development-indicators#
• [Szamil]. (2017). Suicide in the Twenty-First Century [dataset]. Retrieved from https://www.kaggle.com/szamil/suicide-in-the-twenty-first-century/notebook
• World Health Organization. (2018). Suicide prevention. Retrieved from http://www.who.int/mental_health/suicide-prevention/en/
The 12 attributes are namely; country, year, sex, age group, count of suicides, population, suicide rate, country-year composite key, HDI for year, gdp_for_year, gdp_per_capita and generation.
2 | P a g e
In the dataset set there are some attributes which are not familiar to us. HDI stands for “Human Development Index”. It is a statistical tool used to measure a country's overall achievement in its social and economic dimensions.
GDP stands for “Gross Domestic Product”. It is a monetary measure of the market value of all the final goods and services produced in a specific time period, often annually. Then GDP per capita is a measure of a country's economic output that accounts for its number of people. It divides the country's gross domestic product by its total population. That makes it the best measurement of a country's standard of living. It tells us how prosperous a country feels to each of its citizens.


# Methodology.
  1) Problem definition/specification.
The very first step in problem-solving is the identification of a need. There are lots of data in the world which can be useful. So, I am trying to figure out some useful pattern from a dataset which has the data about suicides rates. There are lots of techniques, tools and approaches to mine the data. So, this step helps us to select appropriate data mining tools and techniques to implement the data mining project

  2) Find the related dataset.
There are lots of datasets in the internet. We have selected the most suitable dataset which can be used for out project. It is consisted with more than 27 000 observations with 12 variables.

  3) Data pre-processing task.
The real-world data are dirty. So, we need to expose the best data to out tools to have good results. Initially the data in the dataset are not well formatted. There are some missing values, noisy data and some outliers in the dataset. It is very important to clean the data set when we are doing some analytical purposes using that dataset. So, exposing the dataset into data preprocessing task, is a must thing in order to have a well-structured dataset from existing dataset.
In my dataset the HDI for year attribute has missing values for more than 19k records which makes of around 70% of total number of observations. Because HDI for year is dropped and a separated dataset is created where analysis is done based on HDI. Data is missing for various
countries for various years but in 2016, no suicides data is available for 85 countries. Therefore, the countries which suicide data is available for less than 10 years have been dropped.
It’s very hard to mine patterns or correlations by considering the data country vice. So, continents were mapped to countries. Data for year 2016 is dropped due to very few observations.

  4) Data visualization and analyzation.
Data visualization is the graphical representation of information and data. By using visual elements like charts, graphs, and maps, data visualization tools provide an accessible way to see and understand trends, outliers, and patterns in data. In the world of Big Data, data visualization tools and technologies are essential to analyze massive amounts of information and make data-driven decisions.
Common general types of data visualization:
  • Charts
  • Tables
  • Graphs
  • Maps
  • Infographics
  • Dashboards
Using above common general types of data visualizations and other methods we can do some analytical purposes. We can find correlations among the attributes and dependability on each attribute. Here multiple analysis have been done on grouping data by; age, sex, country, gdp_per_capita and year.


# Technology.
Here I have used python programming language as my main development technology. It is a open-source programming language with a large community. New libraries or tools are added continuously to their respective catalog. Python provides a more general approach to data science. Python is a general-purpose language with a readable syntax. Python can be used for data wrangling, engineering, feature selection web scrapping, app and so on. It is a tool to deploy and implement data mining at a large scale. Python codes are easier to maintain and more robust. Most of data mining tasks can be done with five python libraries: NumPy, Pandas, SciPy, Scikit-learn and Seaborn.
The jupyter notebook has been used as the programming IDE. It is an open-source web application that allows you to create and share documents that contain live code, equations, visualizations and narrative text. Uses include: data cleaning and transformation, numerical simulation, statistical modeling, data visualization, machine learning, and much more. Jupyter notebook has been used as the IDE.

# Implementation.
  1. Import necessary packages.

  2. Read the data from csv file.

  3. Data pre-processing.
    I. Handling missing values.
          In my dataset the HDI for year attribute has missing values for more than 19k records which makes of around 70% of total number of observations. Because HDI for year is dropped and a separated dataset is created where analysis is done based on HDI. Data is missing for various countries for various years but in 2016, no suicides data is available for 85 countries. Therefore, the countries which suicide data is available for less than 10 years have been dropped.
    II. Integrate data and mapping data
          Continents were mapped into countries because it’s very easy and give much more details in big picture.
    III. Data reduction.
          Data for year 2016 is dropped due to very few observations

    IV. Convert columns to categorical data.
          Since I am doing association rule mining, it’s needed to convert numeric data in categorical data in some particular algorithms as well as in some situations.  
 


