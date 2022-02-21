# Chicago Crime Analysis

This project contains an end-to-end data science project about the Chicago crime dataset for the CS 4980 class.

### Datasets
The datasets used in the project include:
* [Chicago Crime Dataset](https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2)
* [NOAA Chicago Weather Dataset](https://www.weather.gov/wrh/Climate?wfo=lot)
* [Chicago Park Dataset](https://data.cityofchicago.org/Parks-Recreation/Parks-Chicago-Park-District-Facilities-current-/5yyk-qt9y)
* [Chicago Library Dataset](https://data.cityofchicago.org/Education/Libraries-Locations-Hours-and-Contact-Information-/wa2i-tm5d)
* [Chicago Public Art Dataset](https://data.cityofchicago.org/Parks-Recreation/Parks-Public-Art/sj6t-9cju/data)


### Hypothesis
1) The likelihood of an arrest can be calculated from the type of crime and weather features.

2) The likelihood of an arrest can be calculated from the type of crime and the crime's location in relation of libraries, parks, and public art.

3) Days with inclement weather will have different amounts of the most common crime (Battery and Theft) than days without inclement weather.


### Results
1) Hypothesis 1 was rejected.  We rejected our alternative hypothesis that the likelihood of an arrest occurring for a crime using the crime type and weather data could not be accurately predicted. However, the crime type and some of the weather features such as percipitation, snow, and temperature were statistically significant compared to an arrest occurring. The significance was not enough to contribute to the predictions of a model.

2) Hypothesis 2 was accepted. We were able to prove and accept our alternative hypothesis that the likelihood of an arrest occurring for a crime was impacted by the crime type and the crime's location in relation to parks, public art, and libraries. Our best model was able to predict arrest likelihood with a 90.3% accuracy. The crime type, crime location, and crimes distance to the nearest park, public art, and library were all statistically significant compared to an arrest occurring.

3) Hypothesis 3 was accepted. We were able to prove and accept our alternative hypothesis that the weather impacts the number of crimes per day for most crimes in Chicago. When looking to predict the number of crimes per day, and the weather of a given day, our models performed very poorly and failed to predict in most cases. This could likely be improved with other data, but when directly analyzing the correlation between weather and crimes, there is little relationship when looking at continuous variables.

The process to arrive at these conclusions can be found within our [final-project.html](./final-project.html) notebook.

### Conclusion
We learned a lot about evaluating hypotheses during this project. Specifically, we had a few ideas of what to look for, but didn't know what to expect. Through our analysis, we found that some of our hypotheses didn't translate to models - making it impossible to generate predictions in some cases. We were able to learn a lot about testing different hypotheses, and working off of what was evaluated. For example, working on hypothesis 3, we figured out that we weren't able to model on the data, however, we were able to derive additional tests (such as looking at the predictive capability of different features) to determine the composition and layout of the data. 

We also were able to learn a lot about R through this assignment. Focusing more on statistical testing in R would have made different areas of this project much easier, but we all feel that we were able to pick up on the assignment relatively fast.
