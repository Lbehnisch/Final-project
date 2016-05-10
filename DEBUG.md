
Debug Log Final Project

Gesture Controlled Midi Controller

1.
I decided to use ultrasonic distance sensor to determine the distance between the sensor and the users hand. 

Instead of the distance the controller is giving me the value for the time it took for the ping to go back and forth. 

I was using the wrong command: 

d = ping();
Serial.println(d);

2.
Having problems of getting readable values in the serial-monitor. 

Adding a delay: delay(250);

3.
Values are still funky and the sensor seems unreliable.

I decide to try a new sensor: The Sparkfun XY Gesture Sensor. 



4.
After installing the Sparkfun Library USB-Port does not get recognized as long as the sensor is connected. 

From my internet research i suppose to be a problem with the NTFS Drivers. 

I install a driver pack which does not solve the problem. 

5. Still having problems with the Drivers

I install an older set of drivers through the terminal. 

USB-Port still is not recognized. 

5. 
I look through the error message and it gives me folder in my finder. 

I suspect a wrong folder in my libraries folder in my finder. 

I delete the wrong folder. 

The sensor works now. 


6. 
Installing hairless midi to send midi to Ableton. 

Hairless midi does not connect to Arduino

I suspect the problem to be in the preferences. 

Hairless midi still does not connect. 


7.
I restart hairless midi after opening Arduino

I receive a signal but pretty random numbers.



8.
I try dividing the numbers from the sensors into values from 0 - 127

Can’t really figure out a good way to do it in code. 

Use constrain instead


9.
Hairless midi  does not show me numbers but signs and letters. 

After long internet research I change the baud-rates in both programs to 115200. 

Hairless midi still shows strange signs in its serial port



10.
Hairless midi still shows signs and letters

After restarting I change the baud-rates in both programs to 9600

Hairless midi shows now numbers. 


11.
After changing a small amount of coder Hairless midi shows signs and letters.

I restart both programs and use only one of the serial monitors. 
(never have both monitors open)
Hairless midi shows now numbers. 


12.
Trying to find the right command in the midi library. 

MIDI.sendNoteOn only sends single note but separate velocities.

13.
Using sendControlChange instead. I used part of a code where someone created a midi controller with potentiometers.

sendControlChange is the right command to change values through the serial monitor that can be mapped inside Ableton.

14. 
I don’t receive any signal inside ableton

I think the problem is that the IAC drivers aren’t turned on yet.
IAC drivers turned on and messages inside Ableton

15.
I want to be abele to change the effect inside Ableton, by changing the channel with the gesture sensor
I bring in the gesture example code.
The code switches to note mode instead of switching the channel
