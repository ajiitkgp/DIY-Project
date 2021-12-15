# DIY-Project
Arduino Traffic Light Controller

Contents

1.Introduction

1.1. Motivation

1.2. State of Art Practices

2.Our model

2.1. Component Description

2.2. Circuit Diagram

2.3. Working of the project

3.Conclusions

3.1. Applications

3.2. Limitations

Introduction

This project presents a working model of a traffic light
employed to regulate traffic at 4-way intersections, realised using
an Arduino R3 board as the controller and coloured LEDs to
represent the lights themselves. It can be easily extended with
pedestrian crossing lights and timer display for real life
application(s).
Motivation:
The motivation for this work is to investigate and interpret
the working of different components of real-life traffic lights and
incorporate it into a small-scale working model. We had also
decided to suggest improvements in the existing traffic light
systems.
State-of-the Art Practices:
During our research, we found that existing traffic light
control systems are quite efficient, making use of complex
equipment consisting of controllers and processors, relays,
control panel with switches, communication ports et cetera.
Some state-of-art traffic regulation systems we encountered
made use of modern solid state computerised systems to regulate
the electromagnetic controllers and clockwork mechanisms for
easy setup and maintenance purposes.
One of the more advanced versions of the controller system
include integrated traffic density monitoring and regulation of
different coloured light intervals accordingly i.e., it shortens/skips
the light rotation for particular lane(s) according to traffic density.
This helps greatly in smooth regulation of traffic, especially if one
of the lanes must tackle greater vehicle density than the other.

Our Model

Component Description:

• Arduino UNO R3 board with USB Cable

• 100Ω 0.25W (5%) Resistor X 12

• 5mm LEDs X 12

• Red LEDs X 4

• Yellow LEDs X 4

• Green LEDs X 4

• Male-to-male jumper wires

• Prototyping board (Breadboard)

• Power source (9V battery)

Circuit Design:

For implementation of traffic lights at a 4-way
intersection, we need three LEDs of Red, Yellow and Green
colours at each lane. All the LEDs were to be connected to
the Arduino UNO’s digital I/O pins through respective current
limiting resistors of 100Ω each.
Note: In the practical implementation of the project, we did not
use the current limiting resistors as the current from each
digital I/O pin of the Arduino UNO is only 20mA. This small
current doesn’t provide enough power for the LED to glow
with discernible intensity. However, it is advisable to use the
current limiting resistors in series with each LED.

Working of the Traffic Light Controller Project:

This project aims to implement a simple traffic light controller
using Arduino UNO, where the traffic is controlled in a predefined timing system. The working of the project is very simple
and is explained below:

1. First Lane 1 gets its Green light turned on and in all the
other Lanes, their corresponding Red lights are turned on.
After a delay of predefined time (say 5 seconds), the
Green light in the Lane 3 must be turned on and the Green
light in the Lane 1 must be turned off.

2. As a warning indicator, the Yellow light in Lane 1 is tuned
on indicating that the red light is about to light up. Similarly,
the yellow light in the Lane 3 is also turned as an indication
that the green light about to be turned on.

3. The yellow lights in Lanes 1 and 3 are turned for a small
duration (say 3 seconds) after with the red light in the Lane
1 is turned on and green light in Lane 3 is also turned on.

4. The green light in Lane 3 is also turned on for the
predefined time and the process moves forward to Lane 4
and finally Lane 2.

5. The system then loops back to Lane 1 where the process
mentioned above will be repeated all over again.

Conclusions


Applications:

• A simple traffic light controller is implemented in this
project with a real chance of expansion.

• An external memory can be interface with the main
controller so that the timings are not fixed during its
programming but rather can be programmed during
operation.

• An efficient traffic light controller system will include a
pedestrian signalling system.


Limitations:

• The project is not suitable for actual implementation but
just a demonstration of the process behind the real time
system.

• Real time traffic light controller systems are generally runtime programmable i.e., the operator can change the
timings of each lane as per the intensity of the traffic in
each lane.

• There will also be a provision for either manual operation
or pre-programmed operation.

• The project implemented here doesn’t include the
pedestrian crossing and pedestrian signalling in to
consideration.
