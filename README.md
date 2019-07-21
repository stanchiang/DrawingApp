# DrawingApp

* start with a reference curve
* user will draw a line attempting to match the curve (we'll call it the drawn curve)
* the drawn curve will be represented by an array of coordinate points 
* each point in the array should be associated with its distance from the start point on the curve as a percent distance from the start point
* map the percent values for each point on the drawn curve to a percent distance from the start on the reference line
* convert the percent distances on the reference line to coordintate points
* given a percent distance value calcuate the distance between the reference line's coordinate point vs the drawn line's coordinate point
* to score the quality of the distance, start with a max attainable score, e.g. a max of 10 points
* the score is "max_score - distance" e.g. if the distance is 3, then the score is 7
* if you have 10 coordinate points, with error distance of 0 each, (i.e. a perfect line); the total score is 100, perfect score