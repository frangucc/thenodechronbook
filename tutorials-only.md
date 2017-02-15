# Installing Noobs & Raspbian OS

```
QR_CODE_BOOTING_NOOBS
```

When you first boot up NOOBS, you’ll get a selection of OSes to choose from. Which operating systems are available depends on which model of Raspberry Pi you are using. For this guide, we’ll stick to the most common OSesoperating systems available on the newest models of the Raspberry Pi. Right now, that’s [Raspbian](https://www.raspberrypi.org/downloads/raspbian/), [OSMC](https://osmc.tv/), [OpenELEC](http://openelec.tv/), [Windows IoT Core](https://developer.microsoft.com/en-us/windows/iot), [RISC OS](https://www.riscosopen.org/).

Which one to in stall depends on you. For now, we'll start with noobs, and that's good, cuz you're a noob.

when you open the pi, insert the SD card that comes with it and follow the instructions on the screen.

![](/assets/noobs4.jpg)

![](/assets/noobs3.jpg)

# Going Headless

```
QR_CODE_GOHEADLESS = [https://www.raspberrypi.org/documentation/remote-access/ssh/unix.md](https://www.raspberrypi.org/documentation/remote-access/ssh/unix.md)
```

\(ONE OF VERY EARLY QR CODES REFERENCED IN THE SCRIPT ONLY SECTION\)

```
hostname -I (from the pi)
ssh@pi<IP> (from the remote machine)
```

username: pi  
password: raspberry

# raspi config

this always fun for things like overclocking, advanced options, changing the passwords, boot options, etc.

sudo raspi-config

The headless part SCRIPT can be found at the end of this section of the script only area of stealth mode.

### SECTION 1 / PART 3 / ACT 1 / PAGE 1

Edit here -&gt; [https://www.gitbook.com/book/frangucc/gamifyed/edit\#/edit/master/script\_only.md?\_k=ur4n6r](https://www.gitbook.com/book/frangucc/gamifyed/edit#/edit/master/script_only.md?_k=ur4n6r)

# Making sure the keyboard works - first ever config edit

[https://www.youtube.com/watch?v=L1F-TxTPyiM](https://www.youtube.com/watch?v=L1F-TxTPyiM)

sudo vi /etc/default/keyboard

# Getting Root

CONTENTS

Commands  
Some basic and more advanced Linux commands  
Text editors  
A selection of text editors available on the Pi  
Users  
Setting up multiple Linux users on your Pi system  
Root  
The root user and the sudo prefix  
Cron / Crontab  
Setting up scheduled tasks  
.bashrc and .bash\_aliases  
Your shell configuration and aliases  
rc.local  
Configuration of initialisation

## The SUPERUSER & PI WITH SUDO

The Linux operating system is a multi-user operating system which allows multiple users to log in and use the computer. To protect the computer \(and the privacy of other users\), the users' abilities are restricted.

Most users are allowed to run most programs, and to save and edit files stored in their own home folder. Normal users are not normally allowed to edit files in other users' folders or any of the system files. There's a special user in Linux known as the superuser, which is usually given the username root. The superuser has unrestricted access to the computer and can do almost anything.

SUDO

You won't normally log into the computer as root, but you can use the sudo command to provide access as the superuser. If you log into your Raspberry Pi as the pi user, then you're logging in as a normal user. You can run commands as the root user by using the sudo command before the program you want to run.

For example, if you want to install additional software on Raspbian then you normally use the apt-get tool. To update the list of available software, you need to prefix the apt-get command command with sudo:

sudo apt-get update

Find out more about the apt commands.

You can also run a superuser shell by using sudo su. When running commands as a superuser there's nothing to protect against mistakes that could damage the system. It's recommended that you only run commands as the superuser when required ,and to exit a superuser shell when it's no longer needed.

WHO CAN USE SUDO?

It would defeat the point of the security if anyone could just put sudo in front of their commands, so only approved users can use sudo to gain administrator privileges. The pi user is included in the sudoers file of approved users. To allow other users to act as a superuser you can add the user to the sudo group with usermod, edit the /etc/sudoers file, or add them using visudo.



# Checklist time. We're about to start with input output in C, but before that, make sure we've done this stuff...

unix safe
who
uname -a
hostname -I
hostname -i
netstat -in

### USERS MUST

* be able to fire up a linux machine or connect to one from a unix or power shell terminal. 
* be able to connect to that machine and transfer files over to that machine using ssh + scp/cat/cp/mv etc.
* run docker and github on the host machine to create a web based portal for hosting their software
* connect their software to the cloud and physical real world devices and store data on AWS
* Run more complicated programs and tasks with electronics and breadboards, gain points and unlock privs the more you register and run services. 

# 6 things to do to a pi after unboxing video


{% youtube %}https://www.youtube.com/watch?v=fLtsXwdM4n0 {% endyoutube %}

----- Installing Raspbian OS
----- Do the SSH into Raspberry Pi 
----- Get the GUI of Raspberry Pi onto Laptop
----- AutoLogin the Raspbian OS for doing Automation 
----- Setup Wi-Fi and Bluetooth of the Raspberry Pi 3
----- Customizing Raspbian OS Panel settings, Desktop Appearence

Download Putty.exe
http://dl1.filehippo.com/371b5381fdcb...

Download VNC Viewer x64 Bit
https://www.realvnc.com/download/file...

Download Win32DiskImager
http://jaist.dl.sourceforge.net/proje...

Download Raspbian Image
http://vx2-downloads.raspberrypi.org/...

Download WinRar
http://www.win-rar.com/fileadmin/winr...

Commands
sudo apt-get update --fix-missing
sudo apt-get install tightvncserver
tightvncserver
sudo apt-get install blueman
sudo apt-get install wicd-gtk

> What this man describes in the youtube video is how to plug your PI in and have it automatically connect to the WIFI on boot with (wicd-gtk) and fire up Bluetooth services with (blueman) so that the PI can both be connected to and connect to other nearby devices. 

Establishing these connections is important. 

# To Kali or not to Kali

kali linux (stay away installation https://www.youtube.com/watch?v=6xXnUGR_e4E

Frank read this is histerical https://youtu.be/ogM69CFbjV4?t=36s

"but they don't even know the shit about the tutorials...."

"their using the aircrackng..." 

Basically, we need to decide what environment we will move to. This book must square away a really great environment where we can go from. 

Is Kali important or not? Is this too deep into penetration testing?

### My official thoughts on this are the minute we go too deep here and get into things like Aircrack, Wifi hacking, etc - the line is crossed from studying IoT/Electronics/Software product making to the ultra specifics of penetration testing and security. This book must direct the hacker mentality (figuring and learning anything out) and apply it to robots, products and software. 

> The fact is that these areas are where things overlap and yes, need to be secure, eventually. You cannot make an IoT product without thinking about handshakes, encryption, passing through wifi (with permission), LoRa/Bluetooth/RF, etc. 

> Despite all this stuff, let's not forget that The Hacker Way should give hackers a well rounded ability to figure any of this stuff out and go really deep in some areas when there is a very specific need. 

# ssh keygen known_hosts SCP has to come in soon

> this is how we connect our macbook pros to ubuntu servers and such we use in the cloud, to hose our APIs, bots, etc. 

# About time for a .bashrc configuration here

> incredibly cool to be able to edit this config file, which runs anytime linux boots. 

# gcc compiler

must install xcode on mac

install command line tools on mac - GET TO A GCC compiler. Must have a GCC compiler - figure it out. here are clues. Google it. 

Teach people how to google stuff. End of day, you need to be able to run 

```
gcc -v
```

-v flag common, does this thing exit ie: 

```
node.js -v
ruby -v

```
xcode-select --install

```

# cool online tool for interpreting code in any language
http://codepad.org/ by sauscelabs
(we should use this on Gamifyeds website)

# do we dive right into something like pointers?

```

    #include <stdio.h>
 
     int func_one() {
         printf("This is function one\n");
         return 1;
     }
 
     int func_two() {
         printf("This is function two\n");
         return 2;
     }
 
     int main() {
         int value;
         int (*function_ptr) ();
 
         function_ptr = func_one;
         printf("function_ptr is 0x%08x\n", function_ptr);
         value = function_ptr();
         printf("value returned was %d\n", value);
 
         function_ptr = func_two;
         printf("function_ptr is 0x%08x\n", function_ptr);
         value = function_ptr();
         printf("value returned was %d\n", value);
     }
 
 ```
