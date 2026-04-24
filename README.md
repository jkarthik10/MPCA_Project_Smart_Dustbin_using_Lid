# MPCA_Project_Smart_Dustbin_using_Lid

Smart Dustbin Lid System

 Overview

The Smart Dustbin Lid System is an automated solution designed to provide a touchless waste disposal experience, improving hygiene and reducing the spread of germs.

This project uses an ultrasonic sensor (HC-SR04) and a servo motor (SG90) controlled by an Arduino Uno to automatically open and close the dustbin lid when a user is detected nearby.

The system works based on ultrasonic wave reflection, where the sensor detects objects within a specific distance and triggers the lid mechanism.

 Features

 Touchless Operation (No physical contact required)
 Ultrasonic Distance Detection
 Automatic Lid Opening & Closing
 Timed Operation (3 seconds delay)
 Fast and Efficient Response
 Improves Hygiene & Cleanliness

Components Used

Arduino Uno (ATmega328P Microcontroller)
HC-SR04 Ultrasonic Sensor
SG90 Servo Motor (Continuous Rotation)
Jumper Wires
Power Supply (9V Battery / USB)

Working Principle

The ultrasonic sensor continuously monitors the area in front of the dustbin.
When an object (like a hand) comes within 20 cm, the system detects it.
The Arduino then triggers the servo motor:
Lid opens
Waits for 3 seconds
Lid closes automatically
The servo uses timed rotation since it is a continuous rotation motor.

Forward rotation → Lid opens
Pause → Waste disposal
Reverse rotation → Lid closes

Pseudocode

START
Initialize Pins: Trig, Echo, Servo

LOOP:
  Trigger ultrasonic pulse
  Measure distance

  IF distance <= 20 cm:
      Rotate servo forward → Open lid
      Wait 3 seconds
      Rotate servo backward → Close lid
      Stop servo

  Wait 100 ms
END LOOP

Applications:

Smart homes
Public places (malls, stations)
Hospitals
Schools & colleges
Offices

Advantages:

Completely touch-free operation
Reduces germ transmission
Simple and low-cost design
Easy to implement and maintain

Future Improvements:

IoT integration (mobile app monitoring)
Automatic garbage level detection
Solar-powered system
Voice control / AI-based automation
Real-time response

Team Members

Ganesh Aroda C
J Karthik
Divyansh Badaya

Conclusion

The Smart Dustbin Lid system provides a practical and efficient solution for hygienic waste disposal. By using ultrasonic sensing and automation, it eliminates the need for physical contact and contributes to cleaner and safer environments.
