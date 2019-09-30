# Micro-mobility Austin, TX: Predicting Trip Distances, Bicycle Return Kiosks, and Scooter "False Starts"
Micromobility data analysis of the City of Austin, TX public data sets rearding their docked bicycle program and on-demand scooters.

"BCycle" references Austin's public bicycle program that relies on fixed bike kiosk to rent and return bikes throughout the city.
"Dockless" references the dockless "on-demand" scooter & bike companies that do not have a fixed pick-up or return location.

After cleaning both datasets, both data sets (but in varying degress) had a significant number of rides that ended 
within the first minute or had traveled no distance. In the case of the dockless scooters specifically, 10% of over five million rides ended with no registered travel distance at all! This observation was termed a "false start"---when a rider activated a trip yet for some reason canceled it and registerd zero trip distance. There was no preexisting feature or explaination in the summary that commented on why this was the case.

The original hypothesis was this observation was not due to randomness and that certain features were directly responsible for a statiscally significant outcome. 

On the BCycle data set, linear and logistic regression models were used to predict the trip duration for the sample. To increase the challenge, multinomial classification models were used to predict the likelihood of which bicycle kiosk a bike would be returned given the starting kiosk location and other factors. Of the 96 kiosks in the sample, Naive Bayes and Random Forest Classifier (RFC) were compared. OLS was used to find the most predictive features, and when tested RFC predicted 15% correctly while Naive Bayes predicted the correct kioks 9% of the time. This outcome was significantly better than expected and opens an opportunity for further analysis to improve the model. 

On the Dockless data set compared four models (RFC, Naive Bayes, Logistic Regression, and XGBoost) to test whether a scooter would experience a "false start" engineered features such as the mileage, number of trips, seasonality, time, and other factors. Of the four, RFC classified best with ~70% certainty. Tuning the hyperparameters did yield improvement, yet this outcome opens an opportunity for more feature engineering to better boost predictability. 

Supporting links:

Bcycle data: https://data.austintexas.gov/Transportation-and-Mobility/Austin-B-Cycle-Trips/tyfh-5r8s
Dockless data: https://data.austintexas.gov/Transportation-and-Mobility/Dockless-Vehicle-Trips/7d8e-dm7r
Dockless city council map w/ numbers: http://www.austintexas.gov/GIS/CouncilDistrictMap/
City of Austin micromobility landing page: https://austintexas.gov/micromobility
City of Austin District Representatives: https://www.austintexas.gov/government
Battery life, source 1: https://www.cnet.com/news/electric-scooters-bikes-dockless-ride-share-bird-lime-jump-spin-scoot/
Battery life, source 2: https://www.washingtonpost.com/local/trafficandcommuting/scooters-we-answer-your-questions-about-this-latest-transportation-trend/2018/11/10/a94b7d94-de03-11e8-85df-7a6b4d25cfbb_story.html?utm_term=.05c93aa0f747
Ojo/scooter vespa info: https://electrek.co/2019/01/22/ojo-electric-scooters/
Veoride range info: https://news.uark.edu/articles/46123/veoride-bikeshare-program-adds-150-new-e-assist-bikes
Scooter lifespan: https://mashable.com/article/escooter-lifespan-shared-new-models/
