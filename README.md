# Micromobility_Austin-Bikes-and-Scooters
Micromobility Data Analysis of Austin, TX using the City of Austin's public datasets.

"BCycle" references Austin's public bicycle program that relies on fixed bike docks to rent and return bikes throughout the city.
"Dockless" references the dockless "on-demand" scooter & bike companies that do not have a fixed location and originate from 
a phone application.

After cleaning both datasets, I noticed in both cases (but varying degress) that there were a significant number of rides that ended 
within the first three minutes. In addtion, ~10% of all 5+ million Dockless rides ended with no travel distance at all!

I hypothesized that this was not a coincidence or a data collection issue. Sure enough, I was able to predict with surprizing certainty 
that the mileage, number of trips, and a few other factors that can be summed up as "wear and tear" had a relationship with the likelihood
of how many "false starts," as I called them, a scooter was likely to experience.

This, and many more insights can be seen in the powerpoint and jupyter notebook for further investigation.

Special thank you to my mentor Mike Ricos who dedicated incredible wisdom, skill, and time to helping me complete this project.
