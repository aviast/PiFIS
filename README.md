# PiFIS
Raspberry Pi + EFIS = PiFIS
---

This project is a "proof-of-concept" to see if it's possible to implement an EFIS using the [Raspberry Pi](https://www.raspberrypi.org/).

## Hardware
I will be using a Raspberry Pi 2 Model B for the implementation. (Ordered!)
I have chosen this hardware because:
* it has a decent graphics capability which will be important for presenting a high-quality display, and
* The hardware specification is more than adequate for what I want to do, but it is still considered "low-end" so there is the potential to upgrade to higher-spec hardware if required.

I will buy a variety of sensors to provide the inputs to drive the EFIS. I don't yet have enough familarity with these systems to know how the sensors will connect to the Raspberry Pi. The [MakerPlane](http://makerplane.org/) project is proposing to use the [CAN-FIX](https://github.com/birkelbach/CAN-FIX-ArduinoLib) protocol for communications but I don't yet understand the need for this.

## Software
I will initially start with the [Raspbian operating system](https://www.raspbian.org/) due to the fact that it should have the highest level of support (e.g. hardware drivers etc.) Down the track I may try to port the software to use [FreeBSD](http://www.freebsd.org/).
The EFIS software will be implemented using the [Go programming language](https://golang.org/).
