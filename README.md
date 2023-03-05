# Budget Friendly Housing in Kings County
## Seattle Metro Area Housing Analysis

### Overview and Business understanding
For this project we'll be taking a look at housing sale data from the King's County Sales dataset, which can be found in kc_house_data.csv. Each record represents a house sale in the Seattle area for the year 2021-2022.  Our Client, a real estate agency, specializes in the elusive mid-range home, and is looking for neighborhoods to target to increase their inventory. Our client would like to target the incorporated areas of Kings County, which as a whole covers roughly 10% of Washington state, and so we'll reduce the size of our dataset to reflect that change.  We'll also keep our eye out for any features that might radically boost home price, such as waterfont properties, or homes adjacent to parks or greenways to provide a list of features or locations associated with inflated pricing- in other words, a "what to avoid". 

### Preliminary Data Analysis
Our first steps were to import our libraries and clean the our data.  This included droping a small number of NaN entries, identifying invalid entries, and starting the process of identifying and elimating outliers.

### Review of Variables and Predictors
With  possible predictors from the original columns, and our engeneered column of 'zip', there were over 26 possibilities to examine.  Using our clients interests, and a variety of tools(correlation matixes, scatterplots and simple linear regression models) we were able to pare down our list to three target predictors that became clear frontrunners for inclusion in our final models:  'zip', 'grade', and 'sqft_living'.    

### Modeling
Using an OLS model we were able to identify the impact of both a homes quality (grade) on the mean price, as well as prove that certain amenities are just too pricey to justify for a midrange home.

### Recommendations

### Limitations
Our model had a large MAE even for home prices, and the plot of our residuals demonstrated imperfect distribution.

### Next Steps
Affordable housing is a challange to find in the best of times, and often neighborhoods with lower housing prices are located nearby inherant health dangers like freeways or large industrial areas, or lack the kinds of amennities that inhance quality of life, like greenspaces and grocery stores. Our next steps would be overlay a map of such amenities or dangers over the neighborhoods we've identified as being our most affordable, to analyze the additional benefits and risks of those neighborhoods and to allow our client to have a fuller understanding of its benefits or disadvantages.
