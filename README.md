# telecom_flooded_cell_test
Arduino based solution for checking flooded battery strings for a 60 minute discharge test and calculate battery capacity run time.

I wanted to make an arduino based solution that would give me a close voltage read on a 52V battery plant.  

What I have so far is a rough sketch that monitors the voltage on the battery string and Serial.prints the voltage measurements at given intervals.

The idea being that when used while having the batteries discharge for 1 hour,  the user will have an idea of what the voltage of the plant was.  This takes more readings within the first 5 Minutes so that the Coop De Fouet can be observed.  This program will also print the Trough and Plateau of the Coop De Fouet aswell.

At 46 minutes in a voltage read is taken and another 10 minutes later at 56 minutes.  So long as the second measurement is less than the first this sketch will calculate the time remaining for the battery string.

