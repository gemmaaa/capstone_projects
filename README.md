# capstone_projects

<em>Contents:</em>

### UNHCR Refugee Data
Using data provided by the UNHCR on asylees and refugees migration from 2000 through 2016, I tried to create models to accurately predict acceptance percentage on a per group basis.

Accompanying slide deck <a href="https://docs.google.com/presentation/d/1wMxDIRes806xUZvFiy-JeE9iJjJdNsCAsewfcvzHAfs/edit?usp=sharing">here</a>.

#### Methodology
Using the data provided by the UNHCR, I used ordinary least squares, Random forest and K Nearest Neighbors regression models to see what features are most indicative of high percentage rates, and attempt to answer three research questions. The resources I am using are pandas and numpy for handling and cleaning the data, matplotlib for visualization, and scikit-learn for modeling.

#### Challenges
Some challenges included missing data, changing categories of data collected over the years, no external information (ie, information on wars or political conflicts that would play a role in this data.

#### Key Results
After analyzing the data and using 3 different models with varying resulting levels of accuracy, it appears that the percentage of acceptance of each group can not be accurately predicted past 63% based solely on the features that I had tested. The research questions posed focused on determining meaningful differences between accepted and rejected groups. It appears that there are not specific features that are highly correlated with accepted or rejected groups, at least in the specific categories I investigated.

#### Next Steps

Though some traits have slightly more correlation with higher acceptance rates, this dataset could benefit from external data in order to create a more accurate and meaningful predictive model.


<hr />

### Blog Authors
Using nltk and spacy, I predicted the author of blog posts from a corpus of blogs of approximately 200 authors.


### Hate in USA
Does the presence of hate groups in a city or a state increase the number of hate crimes in the USA? What patterns of growth or decline are apparent in different hate group categories?

Using data from the FBI and the Southern Poverty Law Center, a hate group watchdog, I set out to analyze patterns of hate groups, hate crimes, and answer these questions. 

The project is split into 4 parts: 
* Summary - if you would like a quick(er) overview of all of the following sections 
* Data import and cleaning - for a closer look at that process
* Data analysis - exploring different aspects of the data, and a little bit of feature engineering
* Modeling - more feature engineering, regression models to predict the number of hate crimes in each category based on features for each city with data

Accompanying slide deck <a href="https://docs.google.com/presentation/d/1VFdocv4I-irsW3vdeQrZLW2UM36mZXTDtR-qYuY6A54/edit?usp=sharing">here</a>

#### Methodology

The aim of this project is to quantify the impact of hate groups presence on crime in their area, and to analyze patterns associated with each hate group and hate bias type on a state and local level from 2004 through 2016 across the USA. Models used in this project include random forest regression, K Nearest Neighbors regression, and gradient boosting regression with multi output regressor. 

#### Challenges

Challenges included organizing and combining the data from multiple sources, cleaning up non standardized names of groups, missing data in places, and categorizations of data changing over time.

#### Key Results

The number of hate crimes in areas with hate groups was higher than the number of hate crimes in areas without. Each hate type had a different trajectory of growth or decline, and some categories were consistently larger over time. Other hate types were newer and growing steadily.

#### Next Steps

Many possible next steps could be taken, but one of these would be using natural language processing techniques, which could yield some interesting results. Analyzing texts produced and published by hate groups, or even their texts shared on their social media presences, could reveal some keywords in their rhetoric. Then, different paths could be taken - for example, articles could be examined for bias, using a count of their keywords as a feature, and perhaps the hate group or hate type it was from could be determined.
