# Android Bluetooth Touchpad
## by Nikolay Kostadinov


#### This project is part of my Bachelor Thesis: "Implementation of a Bluetooth touchpad based on Android OS" at the Chair of Operating Systems, TU Munich. You could download it here. I will direct you to it whenever more information is needed.

# Requirements

1. Android device:

Phone running Android version 2.1 and later
ROOT privileges , See http://en.wikipedia.org/wiki/Rooting_(Android_OS)
Unmodified Bluetooth stack Some manufacturers modify the Bluetooth stack in Android, so the framework will not work there. Ex. HTC Desire has proven not to work!
The framework was successfully tested on Google Nexus One.

2. Computer Host:

Computer running Linux OS. The framework was tested on Ubuntu, but other Linux distributions should also work. It is important they use the BlueZ Bluetooth Stack.
If running Ubuntu it is recommended you install Blueman - Bluetooth utility for Ubuntu with nice GUI. (sudo apt-get install blueman)
Windows will not work! And this is very unlikely to change. Check the thesis, section 5.7.
3. Skills and Knowldge:

Good Android development skills are required. This is not the place to start learning Android.
Good understanding of the Bluetooth stack, HID and SDP is highly recommended. You could read chapter 2, 3 and 4 in the thesis.
Understanding the concept behind the framework is not required in order to utilize its functionality. However, it would be required if you are willing to modify or extend it. You could read chapters 3, 4 and 5 of the thesis.

# Project Contents

1. Bluetooth Touchpad Application

The Bluetooth Touchpad Application is implementing the Bluetooth HID Framework, which could be found in the /src directory and more specifically in the tum.betriebsysteme.kostadinov.btframework package of the project. In the /doc dir you will find the framework documentation. The /jni dir contains the source code of the Linux executable. After compilation the executable file is placed in the /libs/armeabi dir. However, it should be manually moved to the /assets dir, so the SDP component of the framework could deploy and run it. In the /thesis dir one would also find my bachelor thesis as .pdf. Look for the "Videos" section in this wiki to see the app in action.

2. Bluetooth Touchpad Test

To run the Bluetooth Touchpad Test you must first check out the Bluetooth Touchpad Application. By running the test scenarios you could verify if your phone is capable of running the app or not. Read more about it at chapter 7 in the thesis.

3. Sample Code

The sample code project is accompanying the framework tutorial, which could be also found in the wiki. It is the minimum effort required to implement the Bluetooth HID Framework and run a small demo.

# VIDEO

Bluetooth Touchpad Application in action

[![Bluetooth Touchpad](http://img.youtube.com/vi/jT_y4nunPXw/0.jpg)](http://www.youtube.com/watch?v=jT_y4nunPXw)

Check the original Wiki in Google Code: [anroid-bluetooth-touchpad](https://code.google.com/archive/p/android-bluetooth-touchpad/wikis) 
