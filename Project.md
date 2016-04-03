# Final-project
Summary

My goal for this project is to develop a creative and new controller for music producers and Dj’s. Many of the current controllers use potentiometers and faders to tweak parameters, enabling very precise interaction.   The user will be able to interact with the controller without touching. Rather than creating something that is controlling parameters very precisely, this controller is supposed to enable more intuitive and artistic playing. 
3 sensors will be placed on the controller, measuring the linear distance the controller and the hand. This will enable the user to modify 3 parameter with a single movement. The 3 sensors interpret the movement of the hand in a way the user can interact with it in an artistic and intuitive way.  From the Arduino program, the data of the sensors will be send on to the OSCulator. This programm is able to recognize the data from Arduino and transforms it into OSC (open sound controll) data which is almost equivalent to digital midi data.  The user will be able to assign these 3 data strings to the desired parameters in his music program of choice.
The interaction of the user with the sensors will be resembled by several LED which will exist in the controller itself. 

Component Parts

The components I will use are 3 ultrasonic distance sensors, the Arduino UNO and a handful of LED’s. All the components will be hidden inside a 3D printed hull. One will see the LED’s shine through the perforation of the hull. 

Challenges

The most challenging part I think will be to interpret the sensors inside the ARDUINO program in a way, so they give the user a nice and fluid data string inside Ableton. 
Furthermore, sending the data from ARDUINO through OSCulator innto Ableton will be challenging too. 

Timeline

WEEK1
Connecting sensors on the breadboard and gathering data inside the ARDUIONO programm.
Writing the program to collect data from the sensors.

WEEK2
Recognizing the data inside Ableton. 

WEEK3
Finding the right setup for interpretation of the data. 
Connecting the LED’s

WEEK4 
Designing and building  the physical controller.

WEEK5 
Finalizing the design. 
Preparing for presentation.
