#Introduction to Physical Computing

A super-speedy introduction to physical computing for #dhpraxis16
October 19th, 2016
by Mary Catherine Kinniburgh

*huge thanks to Tiffany Chan for her inspiring and helpful [Arduino Tutorial](https://github.com/uvicmakerlab/dhsi2016/blob/master/ArduinoNotes.md) for Digital Humanities Summer Institute 2016, in Jentery Sayers' Physical Computing Class. 

Overview:

What is Physical Computing?

Arduino: 


##Setting up Arduino

1. Take your Arduino and plug in the USB cable to both the Arduino and your computer.

2. Open up Arduino on your computer. Here's what Arduino's logo looks like:

![logo](https://upload.wikimedia.org/wikipedia/commons/thumb/8/87/Arduino_Logo.svg/1280px-Arduino_Logo.svg.png "Arduino Logo")

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


 