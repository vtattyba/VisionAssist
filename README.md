# VisionAssist-

## What is it? 
Designed a User Interface to help people struggling with blindness navigate through their environment. This project utilizes the power TensorFlow and Computer Vision to process camera footage in real-time identifying objects in a user's path. This UI provides haptic feedback through a buzzer to notify if the object is in their path, and which path to take next. 

## Setting Up Pi 
**Raspberry Pi Camera**
- Plug directly into Camera j3 slot Raspberry Pi 4

**Weatherproof Ultrasonic Sensor**
- GND to Pin6(Ground)
- 5V to Pin2(5V)
- ECHO to Pin11(GPIO17)
- Trigger to Pin7(GPIO04)

**Buzzer** 
- GND to Pin14(Ground)
- VCC to Pin4(5V)
- SIG to Pin12(GPIO18)
- NC unused 

## Setting Up Code 
First off all proper API's listed in the code must be installed. Along with this different TensorFlow Models can be used. Currently running 'ssdlite_mobilenet_v2_coco_2018_05_09' as it is optimized. Implementing Google Coral with quantized models will greatly improve performance. 

Execute Object_detection_picamera.py in order to run. 

Code was modified and developed for our own purpose, but initial code was developed by Evan Juras
