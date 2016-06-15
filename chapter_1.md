CHAPTER 1
#  The Raspberry PI 101 - Title TBD

> Introducing the CC sized computer revolution and its amazing applications - insert quote here

Questions from June 2 sessions:

1. What is the PI from a unique separate functionality perspective [web server, coding or prototyping environment, slim linux machine, gpio, general purpose computer/desktop, graphics card [TASK: Definitize this list of things]]
2. What are the different levels of use: [turning on and off, running headless, configuring machine, overclocking, configuration hacks, graphics setups, power libraries, modded OS pi's (kali linux, ubuntu)]
3. What are the genres of projects & experiments: [coding environments, gpio projects, IoT Demos, security pentesting, robotics, artificial intelligence, airplay devices, etc]
4. Can this full spectrum be delivered in a hackifyed gamifyed way?

What's included in the package:

1. 5 Circuit Cards
2. 5 Inspiration Cards
3. Sensors, Resistors, Wires, Breadboard & Sensor Parts [see matrix]
4. Pi Zero or Pi 2 or Pi 3 depending on which one you buy
5. Greeting card with getting started instruction + download app info
6. Comic Book
7. Packaging

| Title | Card # | Parts | Gists |
| -- | -- | -- | -- |
| LED Lights | 1 | 3 Wires, 1 Resistor, 1 LED | 3:2 |
| ADC Conversion w/ Light & Touch | 2 | ADC, Photoresistor, Potentimeter, 7-10 Wires | 3:2 |
| Sound Input & Output | 3 | Mic + Speaker, 6-7 Wires | 3:2 |
| Data Storage, Pipes/Connection/Tunnels & GPS?Streaming | 4 | 2:2 | 3:2 |
| Robot? Power/Motors/AI / Sheild/Breakout | 5 | 2:2 | 3:2 |

## Project Card 1
##### LED Blinking Light Test

1. Materials
2. Tutorial
3. QR Code
4. SKU

## Project Card 2
##### ADC Conversion

1. Materials
2. Tutorial
3. QR Code
4. SKU

## Project Card 3
##### Sound Input & Output

1. Materials
2. Tutorial
3. QR Code
4. SKU

## Project Card 4
##### Working with Data

1. Materials
2. Tutorial
3. QR Code
4. SKU

## Project Card 5
##### Motors

1. Materials
2. Tutorial
3. QR Code
4. SKU

## Inspiration Card 1
##### Vision

1. Tags
2. Symbols
3. Ideas and Clues
4. QR Code
5. SKU
6. Potions

## Inspiration Card 2
##### Mechanics

1. Tags
2. Symbols
3. Ideas and Clues
4. QR Code
5. SKU
6. Potions

## Inspiration Card 3
##### Automation

1. Tags
2. Symbols
3. Ideas and Clues
4. QR Code
5. SKU
6. Potions

## Inspiration Card 4
##### Connections, Clouds & Pipes

1. Tags
2. Symbols
3. Ideas and Clues
4. QR Code
5. SKU
6. Potions


## Inspiration Card 5
##### Machine Learning 

1. Tags
2. Symbols
3. Ideas and Clues
4. QR Code
5. SKU
6. Potions







See notes finish table later...




## Who's using the Raspberry PI

* Pioneering Applications - smaller, cheaper, empowering new apps
* Educational Applications - experiments, GPIO, microcontroller, coding for all, accessibility
* Global world problem solving applications - explore the fields this touches - the interesting work being done world wide with these devices - profile

---
** CHAPTER 1: ** Page 1: TBD

> **PANEL ONE** - TBD

* **Non:** Dude, have you seen the new PI 3?


{% gist id='https://gist.github.com/frangucc/f396c3f501533b6f471f03b82375d737' %}{% endgist %}

{% gistrun id="e57fa69d4697091a20cec1f240bfaa0f" %}
{% endgistrun %}

This is one of my favorite things to talk about. What are they used for today but more importantly, what are they going to be used for more in the near future? What's so great about them?

1. They are much cheaper than a computer and you get a real computer
2. They are unique in their own right because they have a GPIO - laptops and PC's do not offer a GPIO. 
3. CC sized computers with greater processing power, ones like we may see in the very near future enable other equipment used in agriculture, at industry
4. Learning how to minaturize our computers - we're moving backwards to nano and MEMS - which is opening up a whole reange of new applications.

RUSHI: FRANK: TODO: [What are examples of either these chips or IoT suited chips - we are unlocking all this potential]

| GIVE EXAMPLES IN CONTEXT MODEL + RPI 4 & 5 |
| -- |
| TODO: RUSHI & FRANK |



## Intro to PI Hardware - PI 1, 2, 3 and ZERO
> PI 3 Quad Core 1.2 GHZ - half the speed of a new laptop

What are the constants
1. Same style of GPIO programming
2. Still limited by INPUTs and OUTPUTs
3. Video is still limited, can't be in different formats
4. Still need external peripherals
5. All really good learning devices
6. Low memory, low power
7. C compilers
8. Assembly
9. Bluetooth or Wifi or some connection
10. Microprocessor 
11. Architecture (how many registers they are, what IO ports there are, how are they arranged, how is memory accessed, how much memory is internal to the microprocessor, operating voltage) (ARM) and Programming

What are the variables?


---
** CHAPTER 1: ** Page 2: TBD

> **PANEL ONE** - TBD

* **Non:** Dude, have you seen the new PI 3?

* **Gou:** No, but I did just finish creating a PI Zero cluster using Docker. 

* **Non:** What? Where did you get that many PI Zeros, my friends waited in line for an entire day and only could get one! How much did you pay? 

> Non stares at Gou waiting for a reaction. Gou then quielty responds.  

* **Gou:** Promo-codes dummy, I paid five bucks each and bought 50 of em.

#### Basic Diagram of a PI

## PI Setup

| Section Resources |
| -- |
| |


## Operating Systems

An operating system is just a very complicated program. It has the job of organizing other programs on a computer, including sharing the computer's time, memory, hardware and other resources. Some big families of desktop operating systems that you may have heard of include GNU/Linux, Mac OS X and Microsoft Windows. Other devices also need operating systems such as phones, which may use operating systems such as Android, iOS and Windows Phone.

Since the operating system has to interact with the hardware on a computer system, it also has to have specific knowledge of the hardware on a system. To allow operating systems to be used on a variety of computers, the concept of drivers was invented. Drivers are small bits of code that can be added and removed from the operating system in order to allow the operating system to talk to a particular piece of hardware. In this course, we do not cover how to create such removable drivers, and instead focus on making specific ones for the Raspberry Pi.

There are all kinds of different designs of operating systems, and this course can only just scratch the surface. In this course we will mainly focus on getting the operating system to interact with a variety of bits of hardware, as this is often the trickiest bit, and the part for which the least documentation and help exists online.

## PI Performance


> How fast exactly is a PI out of the box


* What can you overclock it to and how to do so (disclaimer)
* Where does it fit in - academically, industrial
* GPIO is digital, no analog is a limitation
* Benchmarking

| Benchmarking Tools |
| -- |
| Nbench  |
| Sysbench |
| Octane |
| Sunspider |
| [https://learn.adafruit.com/introducing-the-raspberry-pi-2-model-b/performance-improvements ](https://learn.adafruit.com/introducing-the-raspberry-pi-2-model-b/performance-improvements )|

NBENCH TEST RESULT EXAMPLE

```
TEST                : Iterations/sec.  : Old Index   : New Index
                    :                  : Pentium 90* : AMD K6/233*
--------------------:------------------:-------------:------------
NUMERIC SORT        :          444.24  :      11.39  :       3.74
STRING SORT         :          36.251  :      16.20  :       2.51
BITFIELD            :      1.2604e+08  :      21.62  :       4.52
FP EMULATION        :          69.824  :      33.50  :       7.73
FOURIER             :          4728.6  :       5.38  :       3.02
ASSIGNMENT          :          6.7648  :      25.74  :       6.68
IDEA                :          1297.9  :      19.85  :       5.89
HUFFMAN             :           654.5  :      18.15  :       5.80
NEURAL NET          :          6.2233  :      10.00  :       4.21
LU DECOMPOSITION    :          228.32  :      11.83  :       8.54
==========================ORIGINAL BYTEMARK RESULTS==========================
INTEGER INDEX       : 19.909
FLOATING-POINT INDEX: 8.599
Baseline (MSDOS*)   : Pentium* 90, 256 KB L2-cache, Watcom* compiler 10.0
==============================LINUX DATA BELOW===============================
CPU                 : 4 CPU ARMv7 Processor rev 5 (v7l)
L2 Cache            :
OS                  : Linux 3.18.5-v7+
C compiler          : gcc version 4.6.3 (Debian 4.6.3-14+rpi1)
libc                : libc-2.13.so
MEMORY INDEX        : 4.228
INTEGER INDEX       : 5.607
FLOATING-POINT INDEX: 4.769
Baseline (LINUX)    : AMD K6/233*, 512 KB L2-cache, gcc 2.7.2.3, libc-5.4.38

```

## Graphics

| Section Resources |
| -- |
| |



## Basic Hello Worlds in All High Level Langs

| Section Resources |
| -- |
| |



## PI Bare metal programming in C

| Section Resources |
| -- |
| [https://www.cl.cam.ac.uk/projects/raspberrypi/tutorials/os/](https://www.cl.cam.ac.uk/projects/raspberrypi/tutorials/os/)|




















