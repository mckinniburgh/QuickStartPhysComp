#A Super-Speedy Intro to Maker Basics with Arduino

*for #dhpraxis16*

October 19th, 2016

by Mary Catherine Kinniburgh

*A big shout-out to Tiffany Chan for her inspiring and helpful [Arduino Tutorial](https://github.com/uvicmakerlab/dhsi2016/blob/master/ArduinoNotes.md) for [Digital Humanities Summer Institute 2016](http://www.dhsi.org/index.php), in Jentery Sayers' Physical Computing and Desktop Fabrication Class. 


#Overview
1. [Why Make?](https://github.com/mckinniburgh/QuickStartPhysComp/blob/master/QuickStart_PhysComp.md#why-make)

   +[Key Term: Maker Space](https://github.com/mckinniburgh/QuickStartPhysComp/blob/master/QuickStart_PhysComp.md#key-term-maker-space)
   
   +[Key Term: Physical Computing](https://github.com/mckinniburgh/QuickStartPhysComp/blob/master/QuickStart_PhysComp.md#key-term-physical-computing)
   
2. [More Speedy Vocabulary](https://github.com/mckinniburgh/QuickStartPhysComp/blob/master/QuickStart_PhysComp.md#speedy-vocabulary)

3. [Setting up Arduino](https://github.com/mckinniburgh/QuickStartPhysComp/blob/master/QuickStart_PhysComp.md#setting-up-arduino)

4. [Activity: Arduino LED](https://github.com/mckinniburgh/QuickStartPhysComp/blob/master/QuickStart_PhysComp.md#activity-arduino-led)

##Why Make?

###Key term: **Maker Space**

Definition: 

*any physical space that offers access to hands-on equipment to produce prototypes of physical objects.* 

_What separates a maker space from a production line (although some large-scale maker spaces have this capacity) is that maker spaces are where you go to *experiment, prototype, and think* with materials_ 

####The process, rather than the product, defines the space.

###Key term: **Physical Computing**

Definition:

Physical computing takes “the human body and its capabilities as the starting point, and attempt[s] to design interfaces, both software and hardware, that can sense and respond to what humans can physically do” (Tom Igoe, “What is Physical Computing”).

+ A popular point of inquiry for critical making and process-oriented prototyping

![physical computing feedback loop](https://github.com/mckinniburgh/QuickStartPhysComp/blob/master/images/interactiveDevice.png)

"The Interactive Device," from Getting Started with Arduino by Massimo Banzi. Borrowed from Tiffany Chan's fabulous Arduino Tutorial

##More Speedy Vocabulary*
*_or how to get started really quickly with some critical making!_

+ *Arduino:* consists of a microcontroller (or programmable circuit board) that comes with software (an IDE) that allows you to write code and upload it to the board. Arduino is an [open source project.](https://www.arduino.cc/en/Guide/Introduction)

+ *IDE:* Integrated Development Environment, or software application with a source code editor, debugging, and other tools. The Arduino IDE is the software that holds your code, as opposed to the Arduino Board, which contains your circuits.

+ *Sketch:* this is Arduino's term for a program--a piece of code that is fed to the Arduino board through USB.

+ *LED:* light-emitting diode. In circuits, diodes make electricity flow in one direction only. This accounts for the importance of *cathode* and *anode* parts of your LED bulb--more on that later!

+ *Resistor:* a device used in circuits that "resists" electricity flow. The [stripes on the resistor](https://learn.adafruit.com/adafruit-arduino-lesson-2-leds/resistors) determine its unit of resistance, measured in ohms. 

+ *Ground:* the reference point from which voltage is measured. 

+ *Breadboard:* a tool for solderless prototyping that makes rewiring simple. 

	For a more thorough introduction to breadboards, see: [https://learn.sparkfun.com/tutorials/how-to-use-a-breadboard](https://learn.sparkfun.com/tutorials/how-to-use-a-breadboard)
	
##Setting up Arduino

1. Take your Arduino and plug in the USB cable to both the Arduino and your computer.

2. Open up Arduino IDE on your computer. Look for this logo:

![logo](https://github.com/mckinniburgh/QuickStartPhysComp/blob/master/images/Arduino.png "Arduino Logo")

3. Set up board

+ Go to "Tools"

+ Select "Board: Arduino/Genuino Uno"
  
      (This is the type of Arduino we're using today)

4. Set up port

+ Go to "Tools"

+ Select "Port"

+ Choose "/dev/cu.usbmodem1411 (Arduino/Genuino Uno)"
	

Now you're ready to make circuits! 

#Activity: Arduino LED

**Supplies**

+ Arduino
+ 2 wires
+ 1 LED bulb
+ Breadboard

**The Circuit**

Don't forget to unplug your Arduino as you wire your circuit! This keeps your computer safe. 

Take 1 wire, and place it in 5V. This is your *ground*.
Take 1 wire, and place it in pin 8. 

Take the *ground* wire to the *cathode* (short side) of the LED on the breadboard. 

On the breadboard, link the *anode* (long side) of the LED to pin 8 with the other wire. Take the wire connected to pin 8 and place it on the breadboard.

![Anatomy of an LED](https://github.com/mckinniburgh/QuickStartPhysComp/blob/master/images/LED-image.jpg "http://sciencewithkids.com/science-facts/facts-about-LEDs.html")

**The Code**

Arduino has ready-to-go code, which we'll use to get started today. You can open their examples and then edit the code as you like. 

1. Go to "File" --> "Examples" --> "01.Basics" --> "Blink"

2. Open the "Blink Sketch," and check out the code. 

3. In "void setup( ), we're going to initialize pin 8 as our output. Change "LED_BUILTIN" to "8".

4. In "void loop( )," change "LED_BUILTIN" to "8" as well. 

5. **Verify** your sketch with the check-mark in the upper-left hand corner of the window
    Troubleshoot: have you selected your proper board and port? Is the Arduino plugged in? If, not check your circuits again. 
    
6. **Upload** your sketch and watch the LED blink!

####Bonus points: change the speed of the LED blinking by adjusting the delay value.     



##Bonus: Arduino Buzzer

1. Go to "File" --> "Examples" --> "02.Digital" --> "toneMelody"

2. Open the "toneMelody" sketch and check out the code. 
 
3. In your supply kit, you'll find a small piezo