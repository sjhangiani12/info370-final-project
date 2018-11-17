 # Project Proposal
Group Names: _Andreas Hindman, Oscar Avatare, Saurav Kharb, Sharan Jhangiani_

## Project Description
_This is a written description of your research project. Depending on the specifics of your project, you should outline the answers to these (and perhaps other) questions:_


- What is the overarching purpose of your research project, and why is it an important undertaking?
>The overarching purpose of this project is to try to predict the size of wildfires. With the current climate in California, this problem is more relevant than ever, and by being able to predict the size of the Wildfire, we’d be able to to better assist in damage control, knowing when to inform individuals to evacuate and where fire containment systems will be needed.

- How does your research fit into the broader problem domain? You should cite at least 3 papers that help contextualize your research.

  >This research topic is becoming more relevant at a concerning rate, as shown by the devastating wildfire events in California this year. Climate change is becoming a more pertinent issue in relation to wildfire rates and severity. The lives of homeowners, firefighters, respondents, and more are in jeopardy due to the unpredictable nature of wildfires.
		https://www.usfa.fema.gov/data/statistics/fire_death_rates.html
        http://science.sciencemag.org/content/313/5789/940
        https://www.theguardian.com/us-news/video/2018/nov/13/camp-fire-deadliest-wildfire-california-history-video-report
        https://www.fs.fed.us/rm/pubs_series/int/gtr/int_gtr030.pdf


- What specific hypothesis (hypotheses) are you going to test?
 >Can fires be accurately predicted by using weather and geographic variables?

- What are the datasets you'll be working with to answer this question? Please include relevant background describing the datasets you identify.
>The data we would primarily be working with contains records of 1.88 Million US Wildfires. This data publication contains a spatial database of wildfires that occurred in the United States from 1992 to 2015. It is the third update of a publication originally generated to support the national Fire Program Analysis (FPA) system. The wildfire records were acquired from the reporting systems of federal, state, and local fire organizations. We would also be collecting associated weather data in order to relate  causes of wildfires to environmental variables.


- What statistical and machine learning methods do you plan on using to test your hypothesis?
>Statistical methods we plan on using are logistic, linear, and multivariate regression. For machine learning models we plan to implement KNN, decision trees, regressions within the fields of supervised and unsupervised learning.  

- Who is your target audience for the resource you will build? Depending on the domain of your data, there may be a variety of audiences interested in using the dataset. You should hone in on one of these audiences.
>The target audience of this resource will be those that are affected by fires or those that want to learn about the impact of fires within certain areas. We imagine this as a tool where users can understand the impact of a fire in their local area by utilizing prior data about fires in similar areas to predict the impact of a fire in this area. With data about the prior size of a fire, we can also take region specific variables and extrapolate the impact to any area chosen depending upon the time of the year and the weather patterns in those areas.

- What should your audience learn from your resource? Consider specific questions they may want to answer.
>The audience should be able to learn the factors that lead to a growth of a wildfire, and thus be able to try and play their part in reducing the exposure to these factors. Ideally, this project will also help them understand and predict how big a fire will grow to, so they are able to prepare and damage control.

## Technical Description
_This section of your proposal is an opportunity to think through the specific analytical steps you'll need to complete throughout the project._

- What will be the format of your final web resource (Shiny app, HTML page or slideshow compiled with KnitR, etc.)?
>The final format of our project would be an HTML report generated using Jupyter Notebook. Interactive data analysis and exploration will be implemented using Shiny app.

- Do you anticipate any specific data collection / data management challenges?
>Getting the Wildfire Data from 1992 - 2015 was fairly simple (converted sqlite file to csv using python). However, we do anticipate some challenges while collecting associated weather data and matching it with our Wildfire data.

- What new technical skills will need to learn in order to complete your project?
>We will probably need to learn new Machine Learning and statistical models (beyond what we were taught in class) that could accurately answer our hypothesis. We hope to get hands-on-experience in implementing and fine tuning ML models. Also working with a data set with almost 2 millions rows should teach us to efficiently handle large datasets.

- How will you conduct your analysis? Please include a detailed description of your intended modeling approach.
>K-nearest neighbours is a non-parametric method used for classification and regression. In this case, we would be using knn regression to find an outcome (fire size) that is the average of the values of its k-nearest neighbours. The input in a knn model consists of k closest training examples in the feature space. We would also be using feature scaling - a useful technique can be used to assign weight to the contributions of the neighbors, so that the nearer neighbors contribute more to the average than the more distant ones.

- What major challenges do you anticipate?
>The biggest challenges we anticipate are within the correlation between disparate data sets to leverage multiple factors to try and predict the size of the wildfires.
