## Smart Pen/Pencil (Assignment 7 Software)

### The Big Picture

<pic>

We decided to pair the pencil along with an android phone. This is becuase of the following
1) To communicate with our web servers
2) Use the microphone in the smartphone to detect when the pen is being used for writing.



### Dpen App

we have developed an android app to help with recording the data sent from the sensors as well as communicate with the web servers.

We have given a start and a stop button to facilitate the start and stop of monitoring the pen.

<pic>


### How it works
When a user wants to use the digital pen, he/she should start monitoring the pen using the start button.This establishes a serial connection with the arduino board as well as starts listening through the mic.
Now when a user writes some data, the accelerometer sends the axis values ( More information regarding this could be found here.) as well as the mic would pic up some sound signals because of using the pen.Both of the above acts as triggers to start recording the values given out by the accelerometer which could then be sent for processing.

<pic>


### Demo
<gif>


### Issues and pending work
1) The amplitude gain observed by the mic is very small, hence chances of getting false positives are high. Need to think of another algorithm to identify the pen usage.
2) Code to send and receive data from the web server needs to be implemented. 
