# Mira Assembly Instructions

## Table of contents

### <a name="Table of contents">Table of contents<a/>

- [Chassis setup](#chassis-setup)  

  - [IO Board](#io-board)
  - [Sata Backplane](#sata-backplane)
  - [Top-IO](#top-io)

- [Motherboard setup](#motherboard-setup)

  - [RAM Installation](#ram-installation)
  - [Drive Installation](#drive-installation)
  - [CPU Installation](#cpu-installation)
  - [Cooler Installation](#cooler-installation)

- [Chassis Installation](#chassis-setupinstallation)
  
  - [MB Installation](#mb-installation)
  - [PSU Installation](#psu-installation)
  - [CPU Duct](#cpu-duct)

- [Imageing and Flashing](#imaging-and-flashing)

  - [Imaging](#imaging)
  - [Flashing](#flashing)

- [Cable Management](#cable-management)

  - [How to manage cables](#how-to-manage-cables)

- [Testing the System](#testing-the-system)

---

## <a name="chassis">Chassis Setup<a/>

### IO Board

![IO Board](/mira-images/IMG_4331-io-board-front.jpeg)

The picture above shows the front of the IO Board that is used in Thelio, Mira, Major, and eventually, Mega. The usage of each header is listed on the IO board, but an explanation of each is below.  

#### FOR MIRA:

FANOUT1/CPU FAN:  
This is used to control the CPU fans. We will have a fan cable running from this header to the top fan splitter.   

FANOUT2/INTAKE FAN:  
This is used to control the bottom intake fan inside the chassis.  

FANOUT3/GPU_FAN:  
This is used to control the add-on we sell as the GPU Fan. If a customer chooses, this fan will go on the GPU brace to intake more air for the GPU. This will use a fan cable to the splitter on the GPU Brace.  

FANOUT4/AUX FAN:  
This is not used by us. This will have a fan cable going to the bottom top (underneath the CPU Fan splitter) for customers to use if they want to add more fans.  

FANIN1/MOTHERBOARD FAN INPUT:  
This will be the input for the IO board to control fans. We will put a cable on the MB CPU Fan header that will go to this input.  

PMB1/MOTHERBOARD:  
This is the power button input from the motherboard. We will use a four-pin cable that has RED and BLACK as LED power, and BLUE and BLACK as the power button actuation input. They are labeled on the IO board and in the MB manual if you ever forget the orientation of POS and NEG.   

PFP1/FRONT PANEL:  
We have Front panel IO but this is not that. This is the rest of the LED and power actuation connections for the power button. It is the same orientation as the PBM1 header. This will go to the power button housing we will install later.  


POWER1/POWER INPUT:
This is a BERG connector header. We will have a Molex cable that needs a converter (which we will put on later) so that we can power the fans on the IO board. This has a clip so if you need to take the BERG connector off, be cautious to not break it.

The last connection on the IO Board is labeled as:  

VBU  
D-  
D+  
GN  

This will be for the USB cable that we will connect from the IO board to the MB. This is used so the OS can communicate with the IO Board to get fan speed readings.

![IO Board Rear](/mira-images/IMG_4333-io-board-rear.jpeg)

This shows the rear of the IO board. There are orange thread protectors that will need to be removed before installation.

The power button is at the far right of the IO Board in this picture. This can be used to turn the system on when the external is off.

[Back to top](#table-of-contents)

---

### SATA Backplane

![SATA Backplane](/mira-images/IMG_4349-sata-bp.jpeg)

The above picture shows the SATA Backplane. We use this to have an additional two SATA drives. This has two SATA cables that will go to the MB. It is powered from the same Molex to BERG connector for the IO Board. The connector is split so it can power both.

---

### Top IO
![Top IO](/mira-images/IMG_4521-top-io.jpeg)

The picture shows the Top IO that the production team installed. This will be connected to the MB. It has a USB-A 3.2 Gen 2, USB-C 3.2 Gen 2, and separate audio in and out ports.

---

## Motherboard Setup

![Motherboard](/mira-images/IMG_4351-mb.jpeg)

This is one of the MBs we use. You can see the CPU socket (covered) in the middle with 4 RAM slots to the right. There are two NVMe covers. All slots are support Gen4 NVMe drives.

[Back to top](#table-of-contents)

### Ram Installation

![Ram Alignment](/mira-images/IMG_4357-mb-ram-align.jpeg)

The above picture shows how to align the RAM with the slot on the board. There is a notch on the DIMM and in the MB slot to prevent previous (or newer) generations of RAM from being used. 

[Back to top](#table-of-contents)

![MB Ram Installed](/mira-images/IMG_4355-mb-ram.jpeg)

In this picture, you can see the RAM slots on the MB. Near the middle above the slots, you can see a diagram. This explains which DIMMs to populate first. RAM is usually able to be daisy chained meaning, you can install two DIMMs, one on each of the two channels, and they can increase total bandwidth. We want this. 

The diagram shows the slots and their names. To the right of the names, it has arrows showing what DIMMs to populate first. If you only have one DIMM, use the lowest alphanumeric which aligns with the DIMMS to use "first".

[Back to top](#table-of-contents)

---

### Drive Installation

![Top NVMe slot](/mira-images/IMG_4358-mb-top-nvme.jpeg)

The picture above shows the top NVMe slot on a motherboard. Remove the heatsink then the plastic covers on the thermal pad. Insert the drive in the slot at an angle, then push the drive down while moving the clip to the side to secure the drive. Once the drive is secure, remove the other plastic cover on the top heatsink's thermal pad and screw in the heatsink.

![Bottom NVMe Slot](/mira-images/IMG_4359-mb-bottom-nvme.jpeg)

Follow the same procedure as the top slot. There will not be thermal pads to install or remove plastic from on for the bottom NVMe slots other than on the heatsink. 

[Back to top](#table-of-contents)

---

### CPU Installation

![MB CPU Cover](/mira-images/IMG_4361-mb-cpu.jpeg)

The above image shows the CPU socket with the cover on. Press the latch down and move it to the left of the CPU socket then move it up.

![CPU open](/mira-images/IMG_4362-mb-cpu-open.jpeg)

![CPU socket](/mira-images/IMG_4363-mb-cpu-socket.jpeg)

When you open the socket, do a quick check to make sure there is no damage. It will be very obvious as the reflections of the pins will look off. If there is damage, please let a manager know and get another MB.  

If there is no damage, place the CPU in the socket. There is a triangle on the CPU. Match this with the triangle on the MP. There are also notches on the CPU that will line up with the socket. 

![CPU Installed](/mira-images/IMG_4368-mb-cpu-installed.jpeg)

Once the CPU is installed, Close the retention cover and move the latch back to the original position. It will take more force with the CPU installed. 

Get the thermal paste from the cooler box and apply it to the CPU as a cross pattern like below.

![Thermal Paste](/mira-images/IMG_4382-cpu-thermalp.jpeg)

[Back to top](#table-of-contents)

---

### Cooler Installation

Take the following out of the box for intel: 

 - Cooler
 - Mounting hardware
 - Extra fans if there  

Take the Intel backplate and move the clips outwards to the 1700 position. The 1700 and 115x positions refer to the Intel CPU socket names. There are many different socket types for Intel and AMD each with their names. You can typically find the socket type on the CPU socket cover, on the retention bracket, and on the MB itself.

![Intel BP](/mira-images/IMG_4370-intel-backplate-rear.jpeg)

[Back to top](#table-of-contents)

---

## Chassis setup/Installation

[Back to top](#table-of-contents)

### MB installation

Make sure all of the cable ties are in place along with the standoffs. Place the MB into the chassis lining up the screws and the IO. 

Once the MB is lined up, screw it in in a cross pattern. Start with the top and bottom middle screws, the left and right middle screws, then the center screw. Then put the top left and bottom right screws, and the top right and bottom left screws. If any of the screws keep spinning instead of tightening, remove the MB and check the PEN insert in the chassis. If the threads look damaged, ask a manager for a new chassis. If the threads look OK, install another standoff and check to see if it spins in the PEM. If it does, ask a manager for a new chassis. If it does not, re-install the MB.

[Back to top](#table-of-contents)

---

### PSU Installation

![PSU Ports](/mira-images/IMG_4401-psu-ports.jpeg)

Take out the power supply and the following cables:

 - CPU power
 - MB power
 - 1x Molex/SATA power
 - PCIe 12vhpwr
 - PCIe power

Plug in the cables BEFORE installing the PSU into the chassis. This is because the PCIe power cable will prevent proper installation. Due to its size, it can hit or sit on top of the intake fan.

Once all of the cables have been plugged in, line up the PSU with the holes on the chassis like below.


[Back to top](#table-of-contents)

---

### CPU Duct

The CPU duct is used to hold fans and direct air flow. Install the fans pointing towards the rear (badge side) of the chassis. 

![CPU Duct Interior](/mira-images/IMG_4520-cpu-duct-int.jpeg)

![CPU Duct Fan Orientation](/mira-images/IMG_4519-duct-fan-ori.jpeg)

Install the duct into the chassis. Line up the chassis brace with the duct and install the brace into the chassis.


[Back to top](#table-of-contents)

---

## Imaging and Flashing

[Back to top](#table-of-contents)

### While the system is imaging:

Please do not stand and wait for the imaging and flashing to complete. You can move on to cable management (section below) while this is happening. Imaging and flashing is an idle process. If something goes wrong while imaging or flashing, you will know and we can address it when it comes up. Otherwise, it can sometimes take 10 minutes to complete. Please multitask.  

### How to

#### Imaging

Imaging the system means you are putting an OS image onto the drive. In this case, we just push a button and it happens for us. We will start with turning the system on. The system should boot into BIOS but if not, the default key to enter BIOS on most systems is 'del'. Press this repeatedly until the BIOS screen shows up. If the screen displayed shows "Easy Mode" you will need to enter "Advanced Mode". Do this by pressing "f7" or "f10". Sometimes this key will be different, but it should be displayed on the screen somewhere.

Once in Advanced, go to the Settings tab. Here, you will see varied options. Look for the selection labeled "IO Ports". In this menu, find Network Stack Configuration, then enable it, then enable IPv4 PXE support. Once it has been enabled, press f10 to save the changes.

The setting we enabled allows the system to boot to an external network device. This device is going to be the trubble station. With Ethernet plugged in, boot the system (if you haven't already) and wait for the trubble-imager to load. Once it is loaded, you will have the ability to select the OS to install (there will only be one) and the drive to install the OS too. If the system only has one drive just press OK to both options and the system will start imaging. 

If you have more than one drive, you will select the OS, but then you will be prompted to choose between the available drives. If they are all the same capacity, choose whatever drive is at the top of the selection. If there are different capacities, the imager will specify what drive the OS should be installed to at the top of the dialog box. Select the proper drive and the rest is the same. Be sure to check that both drives show up in the OS once the system is imaged and flashed.

#### Flashing

This is pretty straightforward. When the system was imaged, it downloaded the BIOS flasher. The boot order is changed so that the flasher will load automatically. Once it is loaded, read through what is on the screen. Most of it you will not need to know or remember. Just follow the instructions. If you press a key other than "Enter" the system will not flash and will instead reboot. We can go back to the flasher by either re-imaging the system, or you can ask a manager for help and they will give you a USB flash drive to boot too.

This will take a few minutes but once done, read through and make sure it didn't fail. Then, press enter and the system will either turn off or reboot. Once the system is back on, it will boot into the OS and display trubble-checklist. This is what you will use to test and ship the system.

[Back to top](#table-of-contents)

---

## Cable Management

[Back to top](#table-of-contents)

### How to manage cables

![Cable Management Rear](/mira-images/IMG_4406-rear-cable-mgmt.jpeg)


This is what the rear of the chassis should look like after doing cable management well. The cables should be flat and neat against the chassis to ensure the external can be put on and removed smoothly.

MB power bundle:

The MB power bundle will contain the UBS-A and USB-C top-io connections, MB power, and Molex power. 

The Molex power connector will use a splitter Molex to Berg cable. This will go from Molex to the IO board and SATA board using the Berg connections. Because the Molex connector has many endings for extra devices, we will rote the extra ends under the MB power cable and the CPU power cable. This will keep the MB power cable bundle from being too large. 

The CPU power cable(s) will meet at the top velcro strap with the CPU fan cable. The CPU fan cable gives input to the IO board. You can see how it is routed in the picture. After going with the CPU power, it will break off and go under the MB power cable. So when the MB power cable is plugged in, thread the cable through the hole between the MB power and MB.

The top-IO cables will go through one velcro loop and then through the thin hole to the left of the MB power cable. This will wrap under the SATA cables and plug into the MB in the respective connectors. The inside view below may help you understand the routing. 

![Internal Cable Management](/mira-images/IMG_4412-int-cb-mgmt.jpeg)

Here you can see how the top-IO cables go under the SATA cables. 

The fan cables that go to the CPU fan splitters will be wrapped inside the chassis like in the above picture. Along with the MB power button cable. The MB power cable will also be wrapped in the bottom velcro that secures the intake fan cable. 

---

CPU power bundle:

For this, you will grab all of the cables coming out of the PSU and use Velcro to tie them together. This will keep the cables from hitting any fans and make things look a bit nicer.

![PSU Bundle](/mira-images/IMG_4409-psu-bundle.jpeg)

[Back to top](#table-of-contents)

---

## Testing the system

[Back to top](#table-of-contents)

Here we will go over how to test the system. The first thing is to go over everything that you have done. Make sure the fans are oriented properly, all of the cables are plugged in and the cable management looks good. Make sure all of the parts are installed. 

In trubble-checklist, you will see a checklist of things to test. 

Video card ports:

For this, you will make sure all of the video-out ports are functional. If the system has a dGPU, you do not need to test the iGPU ports. 

System components:

You will check the included components against what is listed in the checklist. If anything is missing or extra, please let a manager know.

Fan check:

Make sure all of the fans are oriented the right way and that they all work properly. If any of the fans are not working, make sure the IO board is flashed and up to date, and check that all of the fans are plugged into the right headers. You can open Firefox and repeatedly press ctrl + n to open new windows or ctrl + t to open new tabs. This will make the CPU work a bit harder and turn the fans on.

Driver check:

Here we will make sure the firmware is up to date for the MB. Open System76 Driver, make sure the model name matches what you are building and that "All drivers have been applied" is displayed in the lower left of the window. If there are any issues, try imaging and flashing the BIOS again. If the system still does not display the correct model name or has other issues, let a manager know. 

WiFi check:

Here we will open a browser and run a speed test. It does not matter what you use just make sure to be on WiFi and unplug Ethernet. As long as the speed test shows above 300MB/s download and around 200mb/s upload, the system should be fine. Sometimes the internet will be slow, the system may be too far away from an AP, or there is excessive interference that will cause slower speeds. 

Port check:

This will be tested by plugging into all of the available ports (aside from video out) to test that they are all functional. Plug in headphones and open "Sound test". While this is playing you can move the USB for your keyboard around while repeatedly pressing the super key. This will open and close the launcher window. We also want to test USB-C and line-in/mic-in. USB-C NVMe enclosures are floating around Assembly. You may have to ask someone for one. There will also be a microphone floating around that you can test within the sound settings.

Motherboard alignment:

Check to make sure all of the IO lines up with the IO shield. If you passed the Port check without struggling to plug anything in, this should be fine.

Meerkat SD:

If you are not building a Meerkat, skip this.

Do burnin test:

This is a set of stress scripts that are open source and thrown together in-house. If needed, open a terminal and navigate to the Documents folder. Then cd into the stress-scripts folder and run "./s76-burn-in". This will open various windows. Once it is done, you will see a surprised Pikachu with a big "PASS" displayed in the window.

Prepare to Ship button:

If everything is working as expected, type in the serial number of the system, check that it is right, and then press the prepare to ship button. This will set the system up to be used by the customer along with printing a label. Once the system is off, turn it back on and make sure the "Welcome screen" is shown. 

[Back to top](#table-of-contents)
