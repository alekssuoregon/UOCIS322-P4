# UOCIS322 - Project 4 #

Author: Aleksandr Stevens

Contact: alekss@uoregon.edu

Description:
This website offers a system for calculating open and close times for a brevet control based on the input time and distance of the control. 
All interactivity is done using javascript and AJAX. Whenever a new entry is made, the javascript sends the request to the flask server
to run the computation and returns the result as a JSON message. The algorithm used to calculate the open and close times is defined
here https://rusa.org/pages/acp-brevet-control-times-calculator.

Edge Cases:

This part defines special cases not outlined in the rusa.org documentation and how it is handled here.

1.) If the brevet control is at distance 0. Then the open time will be unchanged and the closed time will be +1 hour

2.) If the brevet control is on a boundary(200, 400, 600, 10000), then it will fall within the lower ranges ruleset.

3.) In calcultions, hours are truncated and minutes are rounded up for the open and close times 
