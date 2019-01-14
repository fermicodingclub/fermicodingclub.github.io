---
layout: post
title: "Use cases for Arduino and Raspberry Pi"
date: 2019-01-14 12:00:00 -0600
categories: Arduino RaspberryPi microcontroller web-server
---

# Arduino

From the Arduino website:

> "Arduino is an open-source electronics platform based on easy-to-use hardware and software. Arduino boards are able to read inputs - light on a sensor, a finger on a button, or a Twitter message - and turn it into an output - activating a motor, turning on an LED, publishing something online. You can tell your board what to do by sending a set of instructions to the microcontroller on the board." - [arduino.cc](https://www.arduino.cc/en/guide/introduction)

From SparkFun Electronics:

> "Arduino consists of both a physical programmable circuit board (often referred to as a microcontroller) and a piece of software, or IDE (Integrated Development Environment) that runs on your computer, used to write and upload computer code to the physical board.
>
> The Arduino platform has become quite popular with people just starting out with electronics, and for good reason. Unlike most previous programmable circuit boards, the Arduino does not need a separate piece of hardware (called a programmer) in order to load new code onto the board – you can simply use a USB cable. Additionally, the Arduino IDE uses a simplified version of C++, making it easier to learn to program. Finally, Arduino provides a standard form factor that breaks out the functions of the micro-controller into a more accessible package." - [sparkfun.com](https://learn.sparkfun.com/tutorials/what-is-an-arduino)

There are plenty of Arduino compatible platforms out there and you can often find an equivalent microcontroller for cheaper than the Arduino website. The company Arduino is doing the heavy lifting of designing the system and open-sourcing it.

Here's some DIY projects using Arduinos: [https://www.ubuntupit.com/top-15-best-arduino-projects-that-you-can-build-right-now/](https://www.ubuntupit.com/top-15-best-arduino-projects-that-you-can-build-right-now/)

# Raspberry Pi

> "The Raspberry Pi is a low cost, credit-card sized computer that plugs into a computer monitor or TV, and uses a standard keyboard and mouse. It is a capable little device that enables people of all ages to explore computing, and to learn how to program in languages like Scratch and Python. It’s capable of doing everything you’d expect a desktop computer to do, from browsing the internet and playing high-definition video, to making spreadsheets, word-processing, and playing games." - [raspberrypi.org](https://www.raspberrypi.org/help/what-%20is-a-raspberry-pi/)

The Raspberry Pi is appealing for many reasons including size, cost, and ease of use. Some will reach for it above the Arduino because they can code in Python instead of C++.

Here is a pretty good article that answers many questions: [https://www.makeuseof.com/tag/9-things-wanted-know-raspberry-pi/](https://www.makeuseof.com/tag/9-things-wanted-know-raspberry-pi/)

# Combining tech

## Raspberry Pi is more powerful than Arduino

The Raspberry Pi may seem more powerful than an Arduino and leave you asking why you'd use an Arduino. The answer is, as always, it depends. While the Raspberry Pi has different interfaces for communicating to external devices you may have requirements beyond the Raspberry Pi's capabilities.

Practically, it may make sense for simply use a Raspberry Pi for your project or just and Arduino for your project.

Let's imagine that you have many devices that you want to read, like a [garduino project](https://youtu.be/O_Q1WKCtWiA), and you need fine resolution on the readings, Arduino has more and higher resolution interfaces for these sensors.

We can combine the these two worlds to get the best of both. Arduino as the interface to your electronics and you Raspberry Pi as your interface to your Arduino. The Raspberry Pi could be doing calculations, notifications, database storage, or a web-server all for monitoring the devices attached to the Arduino.

More in this vein: [https://interestingengineering.com/raspberry-pi-and-arduino-whats-the-difference-and-which-is-best-for-your-project](https://interestingengineering.com/raspberry-pi-and-arduino-whats-the-difference-and-which-is-best-for-your-project)
