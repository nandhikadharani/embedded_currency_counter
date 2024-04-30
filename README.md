# embedded_currency_counter
arduino code for smart currency counter
First, include all the libraries in the program. Here we only need the LCD library to be included in the program. Then declare all the variables used in the code.

Inside setup (), print the welcome message on LCD and define all the data directions of digital pins used in this project.
Next, set the output frequency scaling of the colour sensor, in my case, it is set to 20% which can be set by giving HIGH pulse to S0 and LOW pulse to S1.

Inside infinite loop (), read all the data outputs from the sensors.
The output from the IR sensor can be found by reading the A0 pin and output colour frequencies can be found by calling the individual functions written as red (), blue () and green (). 
Then print all of them on the Serial monitor. This is needed when we need to add a new currency to our project.

Here we have only set the conditions for 10 Rupees and 50 Rupees Note color, you can set more conditions to detect more no. of currency notes.
