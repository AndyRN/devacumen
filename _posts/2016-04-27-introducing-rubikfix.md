---
layout: post
title: "Introducing - RubikFix"
comments: true
permalink: introducing-rubikfix
---

As many people know, I have an obsession with Rubik's cubes.

You'll find an array of different types lined up on my desk at work- a 2x2x2, a 3x3x3, a 4x4x4, a 5x5x5, even a <a href="https://en.wikipedia.org/wiki/Megaminx">Megaminx</a>.
<br/><i>In case you were wondering, my current record to solve the 3x3x3 is 46.69 seconds.</i>

On more than once occassion, after someone witnesses me solving one, I've been asked "How did you do that?", usually followed up with "Can you teach me?"... Which got me thinking.

<b>Could I develop an app that can solve a Rubik's cube and detail the process along the way?</b>


## Functionality

In order for the app to actually be useful and not be tiring/cumbersome to use, inputting the state of a cube needs to be smooth whilst taking minimal time to complete.
Rather than entering each face's colour one at a time, I decided that the best way to do this would be by simply taking a photo of it and letting the app do the work. Easy, right?

But, it wouldn't very helpful if the app just went ahead and solved the cube for you, showing how smart the lil' computer is. It would be so much better if there was a way that the cube could be presented to you in it's scrambled state, then be shown step-by-step how to solve it.

Also, a user would need to be able to follow the solve process in a comfortable manner, so it would be nice if the app could have the following features:

* Start/Pause
* Replay last step/Navigate all steps
* Save the user's position in the solve process
* Display the move-list notation of a step/all steps


## Android

I figured the best place to start would be to create an Android app, seeing as I'm already familiar with the OS and that it offers a great deal of flexibility, so I went ahead and downloaded the latest version of <a href="http://developer.android.com/sdk/index.html">Android Studio</a>.

Now it was time to make sure the IDE would recognise my phone in order to deploy the app's code to a device that actually had a camera (The bundled emulators would obviously not suffice).

The phone in question is a OnePlus X that's running Oxygen OS 2.2.1, which is a mobile OS based on Android 5.1.1.

As the phone is not a stock Android phone like the Nexus series, I was skeptical that it would work right away after connecting it to my desktop and launching Android Studio.

<i>Note: In order to develop on an Android device, you'll need to gain access to the 'Developer Options' and enable 'USB Debugging'.</i>


## Getting Set Up

Firstly, I checked to see if my phone was recognised by the IDE:

![RubikFix Connected Devices](/assets/images/android-studio-connected-devices.png)

That's surprising to see. Previously, when developing on other devices, I was faced with driver and compatibility issues which often resulted in disguising the device with a generic Samsung USB driver.

After creating a blank project and punching in the obligatory message, I deployed the app to my phone:

![RubikFix Hello World](/assets/images/rubikfix-hello-world.png)

Now the project can begin!

The first thing I'm going to focus on is getting the camera section of the app right, so that I can input and use real scrambled cubes throughout the development later on, which is what the next post in this series will cover...