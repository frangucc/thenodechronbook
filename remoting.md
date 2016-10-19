Chapter #
# NECK BEARDS

### Operating Systems and Networks

> This section must introduce the modern computer OS foundations and it's filesystems and environments (unix/linux/dos). Booting up a board for the first time is essential and understanding the Linux/Unix and getting around, installing some packages and getting up and running to do some damage is key here. The creators of Linux/Unix/ terminals and bash could be explored. 

Unix - It was developed back in 1969 by AT&T employees working at Bell Labs. Linux came about in either 1983 or 1984 or 1991, depending upon who's holding the knife. The GNU operating system was announced in 1983 by Richard Stallman and started in 1984, while the Linux kernel came about in 1991 courtesy of Linus Torvalds.Mar 24, 2008

The history of Unix dates back to the mid-1960s when the Massachusetts Institute of Technology, AT&T Bell Labs, and General Electric were jointly developing an experimental time sharing operating system called Multics for the GE-645 mainframe. Multics introduced many innovations, but had many problems.

![](https://upload.wikimedia.org/wikipedia/commons/thumb/8/8f/Ken_Thompson_%28sitting%29_and_Dennis_Ritchie_at_PDP-11_%282876612463%29.jpg/1920px-Ken_Thompson_%28sitting%29_and_Dennis_Ritchie_at_PDP-11_%282876612463%29.jpg)

![](https://upload.wikimedia.org/wikipedia/commons/e/ee/Pdp-11-40.jpg)

![](https://upload.wikimedia.org/wikipedia/commons/d/d5/Version_7_Unix_SIMH_PDP11_Emulation_DMR.png)

![](http://sebastien.kirche.free.fr/ordinos/dec/pdp11/pdp11_002.jpg)

![](http://www.saccade.com/writing/projects/PDP11/PanelInCase_Side.jpg)

Ken Thompson, a programmer in the Labs' computing research department, had worked on Multics. He decided to write his own operating system.

While he still had access to the Multics environment, he wrote simulations for the new file and paging system[clarification needed] on it. He also programmed a game called Space Travel, but it needed a more efficient and less expensive machine to run on, and eventually he found a little-used PDP-7 at Bell Labs.[4][5] On the PDP-7, in 1969, a team of Bell Labs researchers led by Thompson and Ritchie, including Rudd Canaday, developed a hierarchical file system, the concepts of computer processes and device files, a command-line interpreter, and some small utility programs.[3] The resulting system, much smaller than the envisioned Multics system, was to become Unix. In about a month's time, Thompson had implemented a self-hosting operating system with an assembler, editor and shell, using a GECOS machine for bootstrapping.[6]

History of the neckbeard.

![](https://upload.wikimedia.org/wikipedia/commons/3/36/Ken_n_dennis.jpg)

![](http://res.cloudinary.com/dzryfxssm/image/upload/v1474555997/neckbeard_rnniog.jpg)

Note that all this led to the MAC OS
Note that Windows called theirs DOS



Show this if needed

![](https://upload.wikimedia.org/wikipedia/commons/thumb/7/77/Unix_history-simple.svg/2000px-Unix_history-simple.svg.png)


**CHAPTER WORKING NOTES**

* Bulleted list of the state of the chapter
* Todos
* ~~Tasks~~


## List of Technical Topics Covered

Before we can start hacking on anything, we need to ensure we have all the proper setup required. 

* Flash the Image
* Boot the PI
* Tour of Terminals & Linux - cheat sheet
* Segway to new tools built on Linux - skip to future -
* Our first BASH Script
* NPM, Node, Setup, IDE Intro
* Hello World (PI)

| Technical Takeaways |
| -- |
| Flash the OS |
| Boot to Root |
| Terminal Cheat Sheet |
| Bash some Packages |
| Node.js |
| NPM |
| Git |
| Hello World PI |
| 0:8 |
| 0:9 |
| 0:10 |

| Axiom Cards Unlocked |
| -- |
| Storage |
| Linux |
| Scripting |
| NPM |
| GIT |
| GPIO |

| Research |
| -- |
| PI Up & Running |
| Arduino Running |
| Environment Tutelage |
| [PI+UNO+Ubidots](https://www.hackster.io/daescobar/arduino-raspberry-pi-ubidots-made-easy-905d51?ref=search&ref_id=raspberry%20pi%20and%20arduino&offset=0)  |

# ART NEEDED...

![](http://placehold.it/800x500?text=KenThompson+Character+Working+Faces)
Ken Thompson character sheet plus working faces... 

![](http://placehold.it/800x500?text=KenThompson+DennisRitchie+working+at+a+PDP-11)
Ken Thompson (sitting) and Dennis Ritchie working together at a PDP-11


![](http://placehold.it/800x500?text=Shoulder+PDP-11)
Over the sholder shot close-up, just like Gou's over the sholder shots on laptop, of the PDP-11


**NOTES!**
SCREENPLAY TO ADD HERE -- need to flesh out this section asap.

GOU doing some serious hacking in unix, the unix cheat sheet -- getting the environments up and running and prepared to really do some hacking projects... SETUP... Need aretwork, bring in the stuff I got... padd around the stuff I got... 


This is where we need to boot up a system - this is where Gou's over should shots, booting the PI and other scenes come into play.

**PI SETUP SCRIPT**

1) I must *FLASH* the OS IMAGE if I want to boot the PI.

2) When I *BOOT* the PI with the IMAGE and hold F7 i get a [LINUX TERMINAL]

3) On Linux, I run [these commands] to get Node.js and NPM installed

4) When I install [GIT] using [NPM] i can then run any open source script or app.

5) When I *clone* a repo with GIT I can run it by following the README

6) If I [Install Gou's Remotify App] I can VNC or Terminal or SSH into my PI and get ROOT access and run any command on the machine I want. [add to Remoting In Chapter]

---

CHAPTER #
# NETWORK ACCESS

> Origins of the internet and networks. Brief history then immediate transition to modern day in Gou Sokyeo's life and knowledge of networks. 

**NOTE: **refactor the raw text below and create a refined set of storyboards and script based on it. Once complete, move to back or appendix. 

ARPANET adopted TCP/IP on January 1, 1983, and from there researchers began to assemble the “network of networks” that became the modern Internet. The online world then took on a more recognizable form in 1990, when computer scientist Tim Berners-Lee invented the World Wide Web.

![](http://worldwebforum.ch/download/attachments/12703568/03_13.jpg?version=1&modificationDate=1463641226643&api=v2)

Sir Timothy John Berners-Lee OM KBE FRS FREng FRSA FBCS (born 8 June 1955),[1] also known as TimBL, is an English computer scientist, best known as the inventor of the World Wide Web. He made a proposal for an information management system in March 1989,[3] and he implemented the first successful communication between a Hypertext Transfer Protocol (HTTP) client and server via the Internet sometime around mid-November of that same year.

erners-Lee was born in London, England,[21] one of four children born to Mary Lee Woods and Conway Berners-Lee. His parents worked on the first commercially-built computer, the Ferranti Mark 1. He attended Sheen Mount Primary School, and then went on to attend south west London's Emanuel School from 1969 to 1973, at the time a direct grant grammar school, which became an independent school in 1975.[1][14] A keen trainspotter as a child, he learnt about electronics from tinkering with a model railway.[22] He studied at The Queen's College, Oxford[1] from 1973 to 1976, where he received a first-class bachelor of arts degree in physics.

"I just had to take the hypertext idea and connect it to the Transmission Control Protocol and domain name system ideas and—ta-da!—the World Wide Web[27] ... Creating the web was really an act of desperation, because the situation without it was very difficult when I was working at CERN later. Most of the technology involved in the web, like the hypertext, like the Internet, multifont text objects, had all been designed already. I just had to put them together. It was a step of generalising, going to a higher level of abstraction, thinking about all the documentation systems out there as being possibly part of a larger imaginary documentation system."[28]

TCP, IP, UDP, POP, SMTP, HTTP, and FTP

Origins of TCP/IP - It is the set of communications protocols used for the Internet and other similar networks. It is named from two of the most important protocols in it: the Transmission Control Protocol (TCP) and the Internet Protocol (IP), which were the first two networking protocols defined in this standard.

History of HTTP - The Hypertext Transfer Protocol (HTTP) is an application protocol for distributed, collaborative, hypermedia information systems. HTTP is the foundation of data communication for the World Wide Web. Hypertext is structured text that uses logical links (hyperlinks) between nodes containing text.

Invention of the IP Address, the internet, TCP/IP/ Protocols, SSH, etc. Only the need to knows that stood up. Intro to UNIX and the first OS systems. 

The hacks in this chapter are about getting into networks such as our own, accessing stuff running on our networks, including our root, the disk, etc. HEAVY on SSH'ing, remote control, even a VNC to finish up. 

> This is an important step in working with modern technology. Get root acces and control of the machines, their IP's, possibly SSH acess, VNC access, access to the code editors, etc.

**Segway to some functional stuff...
**

Ping is the most basic tool we use to check connectivity. We also use arp to check the local broadcast domain and the arp resolution table. traceroute(linux)/tracert(windows) is used to check the path to the destination host. “mtr” is a powerful tool to view the network part for a longer period of time, usually installed as an additional package. Windows version of mtr is also available, even a portable version. One more useful tool comes mostly of out the box is nslookup (windows and linux)  and dig for linux; they are very useful troubleshooting identifying dns related investigation. “whois” is one more tool useful to find out more in some ip or domain name, owner, contact authority, as number etc. Last but not the least netstat available both in windows and linux is a useful tool to find out the local network status easily. A follow the link for a detail tutorial on how to use these basic tools.

![](https://i1.wp.com/farm8.staticflickr.com/7082/7285929392_9b5fe3eb8f_z.jpg?zoom=2)



**Couple notes. Move this. **

The Raspberry Pi has no screen. All the available screens suck right now anyhow. 

We're going to setup a way for our phones to act as our linux shell and remote into our PI's static IP that we give it. 

This is the first major hacking into the PI event. This will be significant. 

**Important Links**
[Remote Control Raspberry Pi](https://www.gadgetdaily.xyz/remotely-control-your-raspberry-pi/)
Use web interface to control PI and get Terminal Access(read or write?)

[Node Wrapper on WPI](https://github.com/gavinhungry/wpi-gpio)
A no-frills wrapper around the WiringPi gpio command-line utility.

[Cams and Linux](http://elinux.org/RPi-Cam-Web-Interface)
Getting cam data and such.

**CHAPTER WORKING NOTES**

* Bulleted list of the state of the chapter
* Todos
* ~~Tasks~~


## List of Technical Topics Covered

Goals for chapter at this point...

* Understand all the relevant protocols and their history
* Get to TCP/IP/HTTP/SSH and give examples in technical and non-technical ways
* 

| Technical Takeaways |
| -- |
| TCP/IP |
| HTTP |
| NETSTAT & others |
| Identify all the network tools that come with linix |
| Understanding packets |
| Understanding SSH |



| Axiom Cards Unlocked |
| -- |
| x |

| Research |
| -- |
| x |



## Screenplay overview, *non-technical*

Description of the non-technical content.

# MAIN SCRIPT A-SIDE
---

TIME, PAGE #'S

** INTRO TEXT ** What time is it, who's here and where are we and what are we doing?

[3 paragraphs]


---

> **NOTES TO ARTIST** Tell the artists what his job is here...

---

**ELEMENTS OF SCREENPLAY**

PAGE # [OVERVIEW]

IMAGES OR SKETCH

SCRIPT ELEMENTS

* **CAP 1:** Captions, Speech, Dialogue

> **PANEL ONE** - ALL CAPS!
> **PANEL TWO** - ALL CAPS!

* **CAP 2:** Captions, Speech, Dialuge

* **BAR 2:** Sidebars, Notes, Pointers




---

## Screenplay overview, *technical*

Description of the non-technical content.

# MAIN SCRIPT B-SIDE
---

TIME, PAGE #'S

** INTRO TEXT ** How does the technical stuff setup... How is it captured, shot, communicated?

[3 paragraphs]

---

> **NOTES TO ARTIST** Tell the artists what his job is here...

---

**ELEMENTS OF SCREENPLAY**

PAGE # [OVERVIEW]

IMAGES OR SKETCH

SCRIPT ELEMENTS

* **CAP 1:** Captions, Speech, Dialogue

> **PANEL ONE** - ALL CAPS!
> **PANEL TWO** - ALL CAPS!

* **CAP 2:** Captions, Speech, Dialuge

* **BAR 2:** Sidebars, Notes, Pointers

Script should feel like this....

* This is where GOU get's into some network hacking stuff... pinging, netstas, ssh, IP addresses, etc. 


Find a clever way to help readers understand these cool tools for networking... (and hacking...)

# Probably do not demo all of this below but do use some of it cleverly and make some reference to other tools you can easily learn once you know the basics.

**tcpdump**

Url: www.tcpdump.org/ category: network sniffer

Description: My favourite tool. No matter where you are if the cable is connected, you will always get some useful info on what’s going on around the network you are connected to.

Howto: I usually start with tcpdump –n –I ethx. I found this tutorial to be helpful http://danielmiessler.com/study/tcpdump/

Available ports: tcpdump usually if a part of any standard linux distribution, it uses libcap library. Some windows version is also available “MicroOLAP TCPDUMP for Windows®”(portable) and Windump.

**tcpdump**

ntop

Url: ntop Category: check network traffic usage with statistics (network statistics generator)

Description: ntop is a network traffic probe that shows the network usage, similar to what the popular top Unix command does. ntop is based on libpcap and it has been written in a portable way in order to virtually run on every Unix platform and on Win32 as well.

Howto: using this tool is straight forward, work pretty much out of the box with minimum configuration. Web based interface makes extracting the statistics easy

Avialable ports for both windows and linux

**ntop**

netsniff-ng

 url http://netsniff-ng.org/ Category: networking toolkit, level: medium to advanced (sniffer)

Description: The netsniff-ng toolkit consists of the following utilities:

netsniff-ng, a high-performance zero-copy analyzer, pcap capturing and replaying tool
trafgen, a high-performance zero-copy network traffic generator
bpfc, a Berkeley Packet Filter (BPF) compiler supporting Linux extensions
ifpps, a top-like kernel networking and system statistics tool
flowtop, a top-like netfilter connection tracking tool
curvetun, a lightweight multiuser IP tunnel based on elliptic curve cryptography
ashunt, an Autonomous System (AS) trace route and ISP testing utility
Howto: Follow the link to find some of the basic commands working in netsniff-ng

Avialable ports: linux only

**iperf**

url  http://iperf.sourceforge.net/ Category: network throughput testing (network throughput)

Description: Iperf is a commonly used network testing tool that can create TCP and UDP data streams and measure the throughput of a network that is carrying them

Howto: it’s a simple tool with a few simple commands like

Iperf –c 192.168.100.1 # to send packet to the server

Iperf –s #run on receiving/server mode

Follow the link for detail guide on iperf

Avialable ports: windows port and linux

 

**wireshark**

Url: http://www.wireshark.org/  Category: Packet analyzer (sniffer)

Description: Wireshark is a free and open-source packet analyzer. It is used for network troubleshooting, analysis, software and communications protocol development, and education. Originally named Ethereal, in May 2006 the project was renamed Wireshark due to trademark issues.

Howto: Usually I have a very simple primitive use for it, most of the time I used to look into tcp/ip packets looking for anomaly while troubleshooting. I found this nice video tutorial on how to use wireshak in detail.

Avialable ports: windows port , linux (redhat)port, other ports

**ethtool**

Url: http://www.kernel.org/pub/software/network/ethtool/ Category: network interface

Description: ethtool is a Linux command for displaying or modifying the Network Interface Controller (NIC) parameters.

Howto: just to display Ethernet driver setting

ethtool eth0

ethtool -i eth0

I found this list useful having a detail usage of this command

Avialable ports linux only

OpenVAS

Url: http://www.openvas.org/ Category: vulnerability scanner (sniffer, scanner)

Description: OpenVAS is a framework of several services and tools offering a vulnerability scanning and vulnerability management solution. OpenVAS was initially named GNessUs as a fork of the Nessus security scanner to allow future free development of the now-proprietary tool.

Howto: If you are used to using Nessus, it is somewhat similar. I found this tutorial to be useful

http://www.unix-tutorials.com/go.php?id=3774

http://www.openvas.org/setup-and-start.html

Available ports: windows and  linux ports

ettercap

Url: http://ettercap.sourceforge.net/ Category: security audit (scanner, sniffer, re-writer)

Description: Ettercap is a free and open source network security tool for man-in-the-middle attacks on LAN. It can be used for computer network protocol analysis and security auditing.

Howto: ettercap is an advanced utility, to use it, one must understand basics of tpc/ip, man in the middle attack, how arp works etc. Check these articles for more on how to use it. http://openmaniak.com/ettercap.php and http://openmaniak.com/ettercap_arp.php

Avialable ports: windows port and  linux port

**netcat**

Url: http://netcat.sourceforge.net/ Category: simple tcp udp read write

Description: Netcat is a computer networking service for reading from and writing network connections using TCP or UDP. Netcat is designed to be a dependable “back-end” device that can be used directly or easily driven by other programs and scripts. At the same time, it is a feature-rich network debugging and investigation tool, since it can produce almost any kind of correlation you would need and has a number of built-in capabilities.

Howto: netcat is simple to use. For example just to open a port on 25 you can use

nc mail.server.net 25

to test if a udp port is open

nc -ul 7000

follow the link for some more fine examples of nc

Available ports: windows port  and linux port

 

**Putty**

url:  http://www.chiark.greenend.org.uk/~sgtatham/putty/ Category: ssh/telnet/tty client

Description: PuTTY is a free and open source terminal emulator application which can act as a clientfor the SSH, Telnet, rlogin, and raw TCP computing protocols and as a serial consoleclient.

Howto: using putty is very straight forward, I don’t think any one used to using any terminal emulator/ssh/telnet client would require much of a help to learn how to use it out of the box. However if you want to use its advanced functions you may appreciate a little bit of help. For more help Putty document page is a good place to start http://www.chiark.greenend.org.uk/~sgtatham/putty/docs.html

Available ports:  windows port . I haven’t seen a Linux port for putty

 NetStumbler

Url www.netstumbler.com/ Category: wireless network scanning

Description: NetStumbler (also known as Network Stumbler) is a tool for Windows that facilitates detection of Wireless LANs using the 802.11b, 802.11a and 802.11g WLAN standards

Howto: use of Netstambler is very intuitive and self explanatory. Its scans the network for access point and the clients and produces a graphical presentation of what it sees. I found this link to be useful http://www.securitytube.net/video/76

Available ports: windows port. Alternatives: Wifi Analyzer runs on android very useful when you want to walk around and survey the network


**nmap
**
url: http://nmap.org/ Category: network security scanner

Description: Nmap sends specially crafted packets to the target host and then analyzes the responses. Unlike many simple port scanners that just send packets at some predefined constant rate, Nmap accounts for the network conditions (latency fluctuations, network congestion, the target interference with the scan) during the run. Nmap has been able to extend its discovery capabilities beyond simply figuring out whether a host is up or down and which ports are open and closed; it can determine the operating system of the target, names and versions of the listening services, estimated uptime, type of device, and presence of a firewall.

Howto: nmap is a medium to advanced level tool. Understanding how tcp/ip works will give you the edge on using this.  To run a simple scan for open tcp port we can use

#nmap –sT 192.168.0.1

#nmap –sS 192.168.0.1 # <=this will run a tcp SYN scan

#nmap –sP 192.168.0.1-255     # <= Ping Scan

Basic usage: http://anish.at.preempted.net/nmap.htm

Reference guide: http://nmap.org/book/man.html

Available ports: windows port and linux port

Angry ip scanner

url: http://www.angryip.org Category: network scanner

Description: Angry IP Scanner (or simply ipscan) is an open-source and cross-platform network scanner designed to be fast and simple to use. It scans IP addresses and ports as well as has many other features.

Howto: usage is simple with a fine GUI, works out of the box every time, basic network skills sets are enough to make use of it.

Available ports: windows port and linux port

**iptraf**

url:  http://iptraf.seul.org/ Category: interface traffic monitoring

Description: iptraf provides statistics on network. It works by collecting data on, tcp/urp/arp connections and provide real-time statistics on activity of the interfaces

Howto: usage is simple and straightforward. All you need to do is run it on an interface. Example

Iptraf –I eth1

Read the manual for more information

http://iptraf.seul.org/2.2/manual.html

Avialable ports: linux port
tag: iptraf, angry ip scanner, nmap, cain and abel, netstumbler, putty, netcat, nc, ettercap, OpenVAS, nessus, ethtool, wireshark, ethereal, iperf, netsniff-ng, ntop, tcpdump, link, download, url, howto, how to, description, 

