# RemoteEV3

RemoteEV3 is a package for controlling a LEGO EV3 robot from a control device, like a laptop or another EV3. Control passes through a network socket, so you can use WiFi or a USB tether.

This project is in early-stage. It only supports the EV3 IR, ultrasonic,and touch sensors.

The goal is to allow a program on a control device to interact with sensors and motors on the EV3, using a programming interface that mimics the MicroPython environment in ev3dev. Tha main use case is for writing MicroPython programs on an EV3 that can control sensors and motors on remote EV3s with the same function names that are used to control devices on the local EV3.

RemoteEV3 is inspired in spirit by NXT-PYTHON https://github.com/Eelviny/nxt-python.

If you are using Python3 instead of MicroPython, you might be interested in RPyC https://sites.google.com/site/ev3python/learn_ev3_python/rpyc.

## Usage Guide

The easiest setup for RemoveEV3 is using two EV3 bricks with ev3dev Pybricks installed. Both EV3 bricks must have a USB WiFi module.

One of the EV3 bricks will be the assistant. The assistant runs the program ev3RemoteAssistant.py and it can have motors and sensors attached to it.

The other EV3 brick will be the commander. The commander runs a MicroPython program that imports ev3RemoteCommander.py. The commander can use the motors and sensors on the assistant.

## Test Programs

Before you can use the test programs, you need to know the IP address of your assistant EV3. Then, in the test program, look for these lines:

    addressList = [
        "192.168.1.122", # WiFi LAN address
        "192.168.0.1"    # USB tethered
    ]

Change the WiFi LAN address to use the address of your assistant EV3.

## Tethering the EV3 Bricks

You can also [tether your EV3 bricks together with a USB cable](https://eltiriel.wordpress.com/2021/10/03/usb-network-with-two-ev3dev-bricks/). This is useful if you participate in a robotics competition where wireless connections are not allowed. 

## Security

The RemoteEV3 package is not secure. It does not use passwords or secure (encrypted) communications.
