# commute
idea for an app that pulls traffic data for a daily commute and generates an overview for IoT/digital assistant applications.


* Home screen interface
* "Record Route" vs "Import Route" vs "Find Route"
* Alternative Routes
* Pit stops (e.g. breakfast, bank, daycare)
* Calendar Sync
* Data View
* Dashboard View
* Hands-free Interface
* Calculate time to destination for Normal Route vs Pit Stops
* Alert thresholds


The MVP for this app is a solution to this use case:
"Alexa, what time do I need to leave to make it to work on time?"

This question assumes that Alexa knows:
* Where you work
* Time to destination based on Google Maps/directions API
* Pulls real-time traffic data from Google Maps
* What time it is
* What time you need to be at work


Out of scope (initially)
* Geofencing your current location (e.g. in the shower adds 10 minutes to estimate)
* Alternative means of travel (e.g. train, bus, plane)



Example query using #commute:

* Alexa, if I want to stop for breakfast, what time do I need to leave for work?

In this example, Alexa needs to add {time to get from Living Room to car and on the road}, {time to Breakfast Restaurant}, and {time to work from Breakfast Restaurant}.  This app can be made simple by requiring a user check-in at the completion of each phase of the journey.  So, in this case, a user might ask Alexa that query, verbally agree "OK, let's do it" (providing the "start the clock" command to kick things off), then check-in once they reach their vehicle, once they arrive at the restaurant, when they leave the restaurant and when they park at work.  Each phase of the journey can now be recorded and averaged against past and future trips -- improving the accuracy of predictions over time.


Why?
This app allows you to query a digital assistant to find out the ETA of your daily commute.

This can already be accomplished clumsily using Google Maps or similar services; #Commute will tailor the inputs to provide personalized information - and also show you longitudinal data about your commute.

The data tracking features could be combined with other datasets, such as vehicle sensor data, other users, weather, etc. to create more nuanced data views.

The overall goal is to minimize travel and be on time.
