# Netflix Exploratory Data Analysis (EDA)
This project investigates patterns in Netflix's catalog to understand what factors play a critical role in Netflix's decision to produce or acquire certain movies or tv-shows. The three factors that will be focused on are: release periods, genres, and maturity ratings. By examining these together, we can discover how Netflix's production strategy and audience targeting shape its media library.

<ins><b>Objectives:</b></ins>
* Are there any spikes in certain genres during a specific season or timeframe?
  * Find periods of content oversaturation or strategic release patterns
* What patterns can be observed between maturity ratings and the lifespan of a TV series?
  * Create insights that inform target age groups for future content

## Tools
These tools were used to quantify trends and visualize how Netflix's content has shifted over time:
* Dbeaver
* SQLite
* Jupyter Lab
* Python: Pandas, Matplotlib, Seaborn

## Dataset
The Netflix_Titles csv datset is from Kaggle, created by the user: **SHIVAM BANSAL**.
* It contains 8807 rows and 12 columns (13 if you count the index column). 
* Out of those fields, these were the primary focus for the EDA's objectives: _type_, _date_added_, _rating_, and _duration_.
* Pre-cleaning was done on Dbeaver using SQLite to handle empty values, duplicate values, and inconsistent fields. The pre-cleaning process can be found inside the EDA. 

## Insights
* No tv-show content was released between the years 2009 and 2012, confirming that Netflix's primary focus is on movie production and acquisitions as show in figure 1 titled, "Netflix Total Content Distribution".
* There was a decline from the year 2019 to 2021 in movies and tv-show production/releases which can be due to external factors such as the COVID-19 pandemic.
* Netflix releases these genres the most for both movies and television: International, Drama, and Comedy. Showing a consistent preference for its platform as noted on both figure 2.1: Netflix Content Distribution by Genre (Movies) and figure 3.1: Netflix Content Distribution by Genre (TV).
* Netflix doesn't follow the expected seasonal trends as it stays consistent in genre releases throughout each season: International, Dramas, and Comedies. However, there are some notable seasonal spikes beyond the top three preferred genres as show by figure 2.3: Netflix Seasonal Content Distribution by Genre (Movies) and figure 3.3: Netflix Seasonal Content Distribution by Genre (TV).
* Netflix continues its patter of targeting a broader audience, as it tries to not focus on more niche or narrower ratings, such as R-rated or TV-Y7-FV per figure 4 titled, "Netflix TV Lifespan per Maturity Rating".

## Preview
<img src="https://github.com/soyshlee/Netflix_EDA/blob/57600dff489d8f02a0ef720fe6f5a0d00fe94e9c/graphs/Figure%201.png" width="700">
<img src="https://github.com/soyshlee/Netflix_EDA/blob/57600dff489d8f02a0ef720fe6f5a0d00fe94e9c/graphs/Figure%204.png" width="700">

## Conclusion
The trends this EDA uncovered, provides a starting point for deeper reasearch into timing, genre patterns, and target audience strategies. Below you will find two possible future endevours to expand on this analysis:
- One pathway of expansion, can be to examine how regional preferences can influence Netflix's decision making around content acquisition/production.
  
- Another direction, would be to study the gap between a title's original release date and the date it was added to Netflix, which could reveal any patterns in important timing decisions. 

# Useful Links
The dataset was retrieved from [Kaggle](https://www.kaggle.com/datasets/shivamb/netflix-shows).

The Jupyter Notebook can be found [here](https://github.com/soyshlee/Netflix_EDA/blob/cd430fe066bec2a860744b9eb742bc557735bfeb/NetflixEDA.ipynb)
