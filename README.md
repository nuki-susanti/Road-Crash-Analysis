# Road-Crash-Analysis

This is python-based project to analyse influential factors causing road crash and to perform predictive analysis of accident severity using classification supervised machine learning. Essentially, the insights drawn could help creating safer environment and less financial loss due to property damage. The data used is a real traffic accidents data collected in South Australia during the year 2021.

# Objective

The objective of this road safety analysis to help analyse the influential factors causing traffic accidents, locate accident hot-spots and perform classification supervised machine learning to predict accident severity. Finally, analysis results and findings are presented using Tableau.
This analysis is therefore divided into two parts:
1. Part 1: Data mining
2. Part 2: Data modelling

# Data

Road crash and casualties data from 2021 in South Australia collected by Department for Infrastructure and Transport. Merged and cleaned data results in 21,242 cases of traffic accidents.
- [Data](https://data.sa.gov.au/data/dataset/road-crash-data/resource/1057e9ae-4672-4123-9c1d-1877483da401?inner_span=True)
- [Data information and dictionary](https://data.sa.gov.au/data/dataset/road-crash-data/resource/02fb14f9-8dcb-4a59-863c-5f7cc3ae1832)
- [South Australian suburb boundaries](https://data.sa.gov.au/data/dataset/suburb-boundaries)

# Tools

The following python libraries were used:
- pandas
- seaborn
- matplotlib
- scipy
- numpy
- geopandas
- folium
- pyproj
- scikit-learn

and also Tableau

# Presentation

[Tableau - Road Crash Analysis](https://public.tableau.com/app/profile/nuki.susanti/viz/RoadCrashAnalysis_16687247255900/RoadCrashAnalysis)


# Conclusion Analysis
### PART 1

<ins>How safe and how severe?</ins>
* Most reported accidents (66%) occur with no injury or casualty, meaning only property damage. The rest of the cases (34.4%) involves casualty.
* Although fatality accounts only for 0.6% of the reported accident cases, it takes the highest of number casualty in average, compared to minor injury and serious injury.

<ins>Time-based analysis: Hourly</ins>
* Generally, accidents occurrence starts to rise in the morning rush-hour and reaches its peak during afternoon rush-hour.
* Fatality cases mostly happen in these two time frames: least crowded time and crowded time.
* Hourly pattern of average casualty of fatality accidents: at 5, 12, 18 and 22.

<ins>Time-based analysis: Daily</ins>
* General pattern occurs during the weekend: Thursday becomes the day of high number of accidents and high casualty, weekend generally shows lower vehicle volumes but increase fatality cases and fatality casualty.

<ins>Time-based analysis: Monthly</ins>
* Generally, accident events of property damage and minor injury remains stable during the whole year and only fatality accident has seasonality.
* In terms of average casualty, interestingly, only fatality has seasonality that reflects three holidays, Easter, summer and winter holidays.

<ins>People-based analysis: Sex, Alcohol & Drugs</ins>
* Ca. 60% of the accidents happens to be male and 40% is female. However, in average, fatality in female (2.24) is higher compared to that in male (1.83).
* Involvement of alcohol and drugs play little role in the number of accidents. 

<ins>People-based analysis: Age</ins>
* The highest number of accident happens with people 20-25 years of age. The number of accidents decreases linearly as a person gets older. 
* Fatality cases are lower for younger people, below 45. 
* Children and very old people are the most vulnerable groups when it comes to injury and fatality, respectively.

<ins>Weather-based analysis</ins>
It is interesting that most accidents happen in the clear weather conditions, opposite to what usually people assume.

<ins>Spatial-based analysis</ins>
* There is indeed accident 'hotspot' where most accidents happen, which is clustered around Adelaide city centre. 
* Most fatalities incidents happened to be in close to the city centre area. *In other words, not only does the complex road system corresponds positively to the number of accidents, but also to the accident severity.*

### PART 2

<ins>Data modelling: Classification</ins>
* One new feature of distance to city center is created.
* Comparing accuracy 3 models: Logistics regression 66.8%, Decision tree 61.8%, Random forest: 74.5%.
Random forest results in distance to city center being the most important feature confirming the previous hypothesis about complex road system of typical city centre.
* Time and location-related characteristics are also listed as important features that also confirm the previous data mining.















