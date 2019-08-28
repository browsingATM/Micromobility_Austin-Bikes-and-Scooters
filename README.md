# Micro-mobility in Austin, TX: How Bike & Scooter Solutions are Performing?
Micromobility data analysis of the City of Austin, TX public datasets rearding their docked bicycle program and on-demand scooters.

"BCycle" references Austin's public bicycle program that relies on fixed bike kiosk to rent and return bikes throughout the city.
"Dockless" references the dockless "on-demand" scooter & bike companies that do not have a fixed pick-up or return location.

After cleaning both datasets, I noticed in both data sets (but in varying degress) that there were a significant number of rides that ended 
within the first minute or had traveled no distance. In the case of the dockless scooters specifically, 10% of all 5+ million rides ended with no registered travel distance at all!

I hypothesized that this was not a coincidence and was worth investigating. Sure enough, I was able to classify with ~70% certainty  whether a scooter would experience a "false start" (as I called them) based on features I engineered such as the mileage, number of trips, seasonality, time, and a few other factors provided by the data set.

Special thank you to my mentor Mike Ricos who dedicated incredible wisdom, skill, and time to helping me complete this project.
