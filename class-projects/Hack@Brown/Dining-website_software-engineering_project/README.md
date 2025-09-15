
PROBLEM: Students often need to decide which dining hall to visit but lack real-time information on 
crowd levels and food quality. It’s inconvenient to walk to a dining hall only to find it overcrowded 
or with subpar food options. Students want a way to view dining hall occupancy, estimate wait times, 
and see feedback on meal quality so they can make more informed decisions about where to eat.

Project Description: Created an end-to-end web-based dining application with the following features: 

* Home: Landing page, can navigate to sections below.
* Reviewer: Can choose a dining hall and submit the occupancy and wait time. Login through Clerk
  is necessary for access (@brown.edu domains only.)
* User: Can choose a dining hall and view the occupancy and wait time. In the case of no available
  occupancy and wait time data from current hour, shows past data.
* Rating Dishes: Can choose a dining hall, the meal and weekend/weekday to view a list of dishes.
  Then users can rate the dishes by pressing thumbs up/down buttons (once per user) and view the average like percentage for each dish. Dish information also includes dietary restrictions and allergens via hoverable icons. Login through Clerk is necessary for access (@brown.edu domains only.)
* Demo button: Sends 3 occupancy and wait time requests every day in a week. We use this
  to demo the predictions.
* Predictions: When most recent data is not found, the user is given the most frequently submitted
  wait time and occupancy for the past week or month depending on availability. Users are informed that the estimate/prediction is not the most accurate.
