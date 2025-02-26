<img src="https://images.prismic.io/homewaterfilters/ad3bbfc0-0d5a-4c3d-b486-9e8df48bbc8f_Calgary_Water_Quality_Canada_City_View_with_Surrounding_Water%5B1%5D.jpeg?auto=compress,format&rect=0,278,1900,710&w=1900&h=710" alt="Calgary Water Source" />

# Analysis of Water Quality in Calgary

This is a comprehensive statistical modelling attempt of Calgary's water pH via physico-chemical properties of water. Specifically for watershed surface bodies of water around Calgary (rivers, streams, reservoirs, etc..).

## About the Data 

The data is sourced from <a href="https://data.calgary.ca/Environment/Watershed-Surface-Water-Quality-Data/y8as-bmzj/about_data">Open Source Data of Calgary</a>. 

**Note:** Please download the full dataset from data.calgary.ca (link above), and select date ranges from 2019-11-26 11:00:00 to 2024-09-05 10:15:00.

## Collaborators and Contributors

This was a course group project. Teammates are listed in the PDF report. 

**Main Contributions**
1. Assisted in modelling
2. Evaluation of the model through multi-linear regression modelling assumptions and statistical tests
3. Scientific Review  

## Analysis 

We were able to produce the following model: 

<img src="images/full_model_equation.png" alt="Model Equation">

The model has an adjusted R-squared 0.5369 with 0.2032 residual standard error. The model explains 53.69% of the variation found in the dependent variable, pH.

## Future Steps 
1. Data pipe-lining: Create a workflow from data.calgary.ca to local environment to contribute towards
2. Consider other modelling methods, multi-linear regression modelling seems to be incompatible with this dataset
3. Further analysis linking results to basic science to harvest more insights from our analysis 
