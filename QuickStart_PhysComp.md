#A Super-Speedy Intro to Maker Basics with Arduino

*for #dhpraxis16*

October 19th, 2016
by Mary Catherine Kinniburgh

*A big shout-out to Tiffany Chan for her inspiring and helpful [Arduino Tutorial](https://github.com/uvicmakerlab/dhsi2016/blob/master/ArduinoNotes.md) for [Digital Humanities Summer Institute 2016](http://www.dhsi.org/index.php), in Jentery Sayers' Physical Computing and Desktop Fabrication Class. 


#Overview
1. [Why Make?](##Why Make)
   +[Key Term: Maker Space](###Key term: **Maker Space**)
   +[Key Term: Physical Computing](###Key term: **Physical Computing**)
2. [Speedy Vocabulary](##Speedy Vocabulary)
3. [Setting up Arduino](##Setting up Arduino)
4. [Activity: Arduino LED](##Activity)

##Why Make?

###Key term: **Maker Space**

Definition: *any physical space that offers access to hands-on equipment to produce prototypes of physical objects. 

_What separates a maker space from a production line (although some large-scale maker spaces have this capacity) is that maker spaces are where you go to *experiment, prototype, and think* with materials_ 

####The process, rather than the product, defines the space.

###Key term: **Physical Computing**

Definition:

Physical computing takes “the human body and its capabilities as the starting point, and attempt[s] to design interfaces, both software and hardware, that can sense and respond to what humans can physically do” (Tom Igoe, “What is Physical Computing”).

+ A popular point of inquiry for critical making and process-oriented prototyping

!["The Interactive Device," from Getting Started with Arduino by Massimo Banzi. Borrowed from Tiffany Chan's fabulous Arduino Tutorial](QuickStartPhysComp/images/interactiveDevice.png)

##Speedy Vocabulary*
*_or how to get started really quickly with some critical making!_

Arduino: 
IDE:



##Setting up Arduino

1. Take your Arduino and plug in the USB cable to both the Arduino and your computer.

2. Open up Arduino on your computer. Here's what Arduino's logo looks like:

![logo](QuickStartPhysComp/images/Arduino.png "Arduino Logo")

3. Set up board
   *Go to "Tools"
   *Select "Board: Arduino/Genuino Uno"
      (This is the type of Arduino we're using today)

4. Set up port

	*Go to "Tools"
	*Select "Port"
	*Choose "/dev/cu.usbmodem1411 (Arduino/Genuino Uno)"
	
Now you're ready to make circuits! 

#Activity: Arduino LED

**Supplies**

*Arduino
*2 wires
*1 LED bulb
*Breadboard

**The Circuit**

Don't forget to unplug your Arduino as you wire your circuit! This keeps your computer safe. 

Take 1 wire, and place it in 5V.
Take 1 wire, and place it in pin 8. 

Take the wire connected to 5V and place it on the breadboard. Line this up horizontally with the longer end of the LED pin. 

Take the wire connected to pin 8 and place it on the breadboard. Line this up horizontally with the shorter end of the LED pin. 

**The Code**

Arduino has ready-to-go code, which we'll use to get started today. You can open their examples and then edit the code as you like. 

1. Go to "File" --> "Examples" --> "01.Basics" --> "Blink"

2. Open the "Blink Sketch," and check out the code. 

3. In "void setup(), we're going to initialize pin 8 as our output. Change "LED_BUILTIN" to "8".

4. In "void loop()," change "LED_BUILTIN" to "8" as well. 

5. **Verify** your sketch with the check-mark in the upper-left hand corner of the window
    Troubleshoot: have you selected your proper board and port? Is the Arduino plugged in? If, not check your circuits again. 
    
6. **Upload** your sketch and watch the LED blink!

####Bonus points: change the speed of the LED blinking by adjusting the delay value.     



##Bonus: Arduino Buzzer

1. Go to "File" --> "Examples" --> "02.Digital" --> "toneMelody"

2. Open the "toneMelody" sketch and check out the code. 
 