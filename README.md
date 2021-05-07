# UOCIS322 - Project 4 #

Author: Aleksandr Stevens

Contact: alekss@uoregon.edu

Description:
This website offers a system for calculating open and close times for a brevet control based on the input time and distance of the control. 
All interactivity is done using javascript and AJAX. Whenever a new entry is made, the javascript sends the request to the flask server
to run the computation and returns the result as a JSON message. The algorithm used to calculate the open and close times is defined
here https://rusa.org/pages/acp-brevet-control-times-calculator. 
