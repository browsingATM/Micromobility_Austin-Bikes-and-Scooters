# Micromobility_Austin-Bikes-and-Scooters
Micromobility Data Analysis of Austin, TX using the City of Austin's public datasets.

"BCycle" references Austin's public bicycle program that relies on fixed bike docks to rent and return bikes throughout the city.
"Dockless" references the dockless "on-demand" scooter & bike companies that do not have a fixed location and originate from 
a phone application.

After cleaning both datasets, I noticed in both cases (but varying degress) that there were a significant number of rides that ended 
within the first minute. In the case of the dockless scooters specifically, 10% of all 5+ million rides ended with no registered travel distance at all!

I hypothesized that this was not a coincidence and was worth investigating. Sure enough, I was able to predict with surprizing certainty 
that the mileage, number of trips, seasonality, time, and a few other factors had a relationship with the likelihood of how many "false starts" (as I called them) a scooter was likely to experience in the future.

Special thank you to my mentor Mike Ricos who dedicated incredible wisdom, skill, and time to helping me complete this project.
