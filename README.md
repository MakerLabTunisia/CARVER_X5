
# CARVER  X5, the Open source 5 Axis CNC Machine

# Story:

## MakerLab :

MakerLab is a Tunisian tech startup specialized in developing customized embedded systems and mechatronics projects to industrials. 
In MakerLab, we believe in the Open Source Hardware philosophy and we want to spread the tech knowledge we gain, with the community so everyone performs itself and benefits from others experiences. And this is why, we made from our little space in Sousse, a **TechSpace**, open for everyone who wants to work on real projects, finding all what a Maker needs to create his own tech project. 
In our TechSpace, many projects were developed and created, even if it is by our staff or by students from different universities across the country, starting from Drones, Internet of Things (IoT) devices, arriving to Robotic Arms and CNC Machines. 
Moreover, this 5 Axis CNC Machine, is our first Open Source Hardware Project we made, and which we are so happy sharing it with the community. 
You can find more details on our TechSpace in our:  
Lien Facebook : https://www.facebook.com/tunmakerlab/
Lien siteweb : https://makerlab.tn/

## MakerLab vision :

We dream in a future of freedom, where open source hardware and MakerLab enable people to fully understand how to make things they need, and where decentralized local production is customized to impact the surrounding community. Believing that empowering the user with knowledge about how to make machines, Carver X5 wants to give to the world a powerful open source tool. And this Machine is one of the first steps in developing other machines sharing the same philosophy.

## Presenting the project:

This 5 axis CNC machine, is part of a big project made by our partners Open Lab Hamburg from the Helmut Schmidt University in Germany, for the benefit and with the collaboration of FABLAB ENIT (National School of Engineering of Tunis), and sponsored by the BMBF. 

<div align="center"><img src="img/image002.jpg" width="50%"></div>
<div align="center"><i>Machine Building Workshop</i></div>
This project consists of organizing a one-week workshop for building machines, and we, MakerLab’s staff, happily and gladly are a part of this first of its kind project in our beloved country, Tunisia.

# Why a 5 axis CNC Machine?

Being always updated to the latest OSHW projects in the community, we found that there is many 3 Axis CNC machines, 3D Printers and Laser Cutter with a very good documentation, but not enough OSHW 5 Axis CNC machines and not at all for the Head/Head. 



<div align="center"><img src="img/image004.jpg" width="80%"></div>
<div align="center"><i>CARVER X5 Machine</i></div>
So we thought we could create the first OSHW, Head/Head, double swivel head form, 5 Axis CNC Machine. We tried our best to make it both robust and easily replicable machine. Constructed mainly from Heavy Aluminum Extrusion profiles, and thick aluminum milled parts HGR25 Linear guides, using NEMA23 Stepper motors, and Rack and pinion for transmission, Carver X5 is capable of milling materials like wood, plastics and soft metals like Aluminum and brass.

# CARVER X5 Machine

## 1. Specifications

**Dimensions 5xm600** 		   : 650 x 670 x 480mm
**Working volume 5xm600**   : 990 x 780 x 1000mm
**Max travel speed XYZ**		: 15000mm/min (X,Y);     3000-6000mm/min (Z)
**Max travel speed BC**          : 20rpm(C)  20rpm(B)
**Motors used**                         : NEMA 23 ( X / Y / Z / B / C)
**Linear guides**                       : HIWIN High accuracy Rails and Blocks
**Structure material**             : Anodized Aluminum 
**Protection**                            : 5mm Acrylic enclosure
**Power requirements**         : 1200W, 240-100V, 50/60hz, 13A 
**Weight**        	           		    : 93kg
**Computer interface**           : USB
**Computer requirements**  : Windows operating system with Mach3    
**Controller**                             : MACH3 (to be purchased separately from an official vendor)
**Software**                               :  supports any CAD/CAM software 


## 2. Machine design

CNC machines are commonly known that they are nothing more than automated robots, their famous type, is a 3 axis CNC machines, which are considered as 3P robots (robot with 3 Prismatic Joints linked with 4 Links). 

But in 5 axis CNC machines we talk about 3P2R robots, because they are composed of 3 Prismatic Joints succeeded with 2 Revolute Joints, and linked with 6 Links.

<div align="center"><img src="img/carver_x5.jpg" width="100%"></div>

<img src="img/carver_X5.jpg" alt="img" style="zoom:50%;" />

<div align="center"><i>CARVER X5 Design</i></div>

Our Joints are named (X, Y, Z, C & B)

The Links are named (Frame, Y2X Bridge, X2Z, Z Axis, C Axis, B Axis in which will be installed our end effector).

## 3. Machine composition:

### ▪ Frame 

Designed to be easily made, assembled and disassembled, we choose the aluminum profile to be the main structure composition.
As it's important that the structure be stiff and robust, we wanted to work with 45 series aluminum profiles.



<img src="img/frame.jpg" alt="img" style="zoom:50%;" />

<div align="center"><i>Machine Frame</i></div>

The machine frame contains the rails and transmission rack of the Y-axis that will carry the other entire axis, this is why we worked with the 45x90 aluminum profiles in the top stage.
The frame carries the mechanical stops; they include a screw to adjust the limit position.

### ▪ Y2X Bridge

The Y2X Bridge is the second link in our 5-axis CNC machine, it links the Y and X joints.

<img src="img/bridge.jpg" alt="img" style="zoom:50%;" />

<div align="center"><i>Y2X Bridge</i></div>

Constructed from two perpendicular 45x90 aluminum profile and two 15mm aluminum plate flanks on which will be installed the Y-axis sliding blocks.

### ▪ X2Z 

X2Z, as its name indicates, do the function of the joint between the two prismatic axis, X and Z.
X2Z is an assembly that plays a big role in our 5 Axis CNC Machine, because it assures both, the linear guiding of X axis, Z axis and their transmission organs.

<img src="img/x2z.jpg" alt="img" style="zoom:50%;" />

<div align="center"><i>X2Z</i></div>

Built totally from thick aluminum plates, X2Z contains the sliding blocks of X-axis installed on its back, and those of the Z-axis, installed between the two X2Z flank plates.
On the X2Z assembly, get installed the X Motor Module and the Z-axis ball bearing Nut.

###  ▪ Z Axis

The Z-axis, slides on the 2 blocks installed on the X2Z Flank plates. The motor module installed on its top assures its motion. The Z motor transmit rotation to the ball screw that moves the Z-axis up and down.



<img src="img/z_Axis.jpg" alt="img" style="zoom:50%;" />

<div align="center"><i>Z Axis</i></div>
In its bottom is installed the swivel head that rotates the end effector in 2 axis.

###  ▪ Swivel Head

The swivel Head is composed from the last two revolute joints, C & B.
What is special about this assembly, is the fact that it should be the more compact possible. So the two motors, their transmission system and even the limit switches and connectors should all be enclosed in this assembly, and this was the hardest task that we encountered in the whole machine design.
While designing the Swivel Head, there was 2 big challenges, the choice of transmission system and minimizing joints offset relatively to each other.

<img src="img/swivel_Head.jpg" alt="img" style="zoom:50%;" />

<div align="center"><i>Swivel Head</i></div>

The first challenge is because C and B axis will handle big effort while milling, and if mounted directly on the motor shaft or even through a reversible transmission system, this may cause a loss in steps when encountering big efforts. This obliged as to work with worm gear, which is an irreversible transmission system.
This choice will cause that the joint offsets get bigger, so we preferred to add a pulley transmission system before the worm gear to prevent the swivel head of getting much bigger.


### ▪ Spindle Motor

For the spindle motor, we did our best to find small and powerful, and not too expensive ones in the market, but we found none.
The main specification needed is a small size, but the most of powerful spindles are so big that you cannot integrate in the swivel head.
This is why we designed and fabricated our own spindle composed of a 540W Brushless motor, a bearing housing and an ER11 chuck.

<img src="img/spindle.jpg" alt="img" style="zoom:50%;" />

<div align="center"><i>Spindle Motor</i></div>

The spindle motor is capable of a max velocity of 20000 RPM at 24V, and has enough torque for milling wood and plastics.

### ▪ Motor Modules

Machine movement along X, Y and Z Axis is assured by 4 motor modules.  Containing pulley and belt transmission system between the motor shaft and the shaft.



<img src="img/y_Module_Motor.jpg" alt="img" style="zoom:50%;" />

<div align="center"><i>X/Y Axis Motor Module</i></div>
<img src="img/z_Module_Motor.jpg" alt="img" style="zoom:50%;" />

<div align="center"><i>Z Axis Motor Module</i></div>

## 4. Electronic enclosure

Installed in an industrial **[plastic enclosure](http://www.akisplastik.com.tr/en-us/Product/ProductCategoriesDetail?categoryId=12)** (400x500x240), the **electronics** of the **CARVER X5** is composed of a set of drivers for each motor including the spindle driver, a USB interface control board, a sensor interface board and two 12v 42A DC Power Supply. 

![img](img/image020.jpg)

​     

▪ **THE PoKeys57CNC control board**
PoKeys57CNC USB and Ethernet CNC controller is a blend between general purpose PoKeys device and motor controller. The device is targeted primarily for controlling up to 8 STEP/DIR signal driven motors (stepper motors, servo drives, etc.) in various applications with the addition of powerful PoKeys device features. 

![img](img/image022.jpg)

 Download PoKeys57CNC datasheet [here](https://www.poscope.com/wp-content/uploads/downloads/Pokeys/Manuals/PoKeys57CNC%20user%20manual.pdf).

▪ **Drivers**
TB6600 Stepper Motor Driver is an easy-to-use stepper motor driver, which could control a two-phase stepping motor. It is compatible with Arduino and other microcontrollers that can output a 5V digital pulse signal. TB6600 arduino stepper motor driver has a wide range power input, 9~42VDC power supply. And it is able to output 4A peak current, which is enough for the most of stepper motors. The stepper driver supports speed and direction control. You can set its micro step and output current with 6 DIP switch.

Download TB6600 datasheet [here](http://olimex.cl/website_MCI/static/documents/TB6600_data_sheet.pdf).

▪ **The sensor cables gatherer board**
The need for the sensor cable gatherer board has emerged due to the multiplicity of sensors. And to minimize the number of cables passing through the cables carrier, we managed to gather them in a 15 cores VGA cable. This board provides the current and voltage needed to all the 11 sensors used in the machine, and is installed on the Y2X Bridge in between the two cables carrier. 

![img](img/image024.jpg)

At the beginning, we used a VGA port but we found a lot of the issues while soldering the 15 cores cables in the VGA port. This is why we managed to use two Ethernet cable which easier to install.

(Board KiCAD)

▪ **The sensors interface board**
This board will play the role of the interface between sensors signal coming from the first board and the pokeys57cnc board through a little circuit of signal adaptation.
 Inductive proximity switches works with 12V power supply, and returns a 12V digital signal, but the pokeys57cnc can only handle 5V digital signal in limit switches inputs. 

![img](img/image026.jpg)

This is why we used a circuit based on a 470 ohm resistor for current limiting and a 5.1V zener diode to let only the needed 5V pass to the control board for each signal. On this map, the extremities and minimum limits (x-min, y-min, z-min) will be connected. 

▪ **Spindle motor Driver**
As we created our own spindle based on brushless DC Motor, we used its recommended Electronic Speed Controller as a driver. A 60A ESC is responsible of driving the motor at 20 000 RPM at 24V.
Product page [Link](https://www.overlander.co.uk/overlander-xp2-60a-sbec-brushless-esc-rtf-speed-controller.html).



## 5. Wiring

 One main task we did is the wiring, and it is so important.
 We used RGB 4 wire Cables for the stepper motors, they thick enough to carry the needed current.
 The end stop switches cables were long enough to reach the first interface board installed on the bridge assembly.
 We gathered all sensors signals in two ethernet cables to facilitate connection.
 Of course all these cables needed a way to be placed in, so we used 57x25 industrial cable carrier to arrange all wires to the electronic enclosure.

 

## 6. Software

### ▪ Fusion360 : CAM software
Fusion 360 combines industrial and mechanical design, simulation, collaboration, and machining in an integrated concept-to-production toolset.
Fusion 360 is the first 3D CAD, CAM, and CAE tool of its kind. It connects your entire product development process in a single cloud-based platform that work both on PC and MAC.

Download [Link](https://www.autodesk.com/products/fusion-360/students-teachers-educators).

### ▪ Pokeys Software : Software for the CNC Interface Board
PoKeys software setup package contains PoKeys configuration tool (also used for firmware updating), USB drivers, manuals, PoBlocks tool, Mach3 plugin etc. After installation, run the PoKeys application to update the firmware of PoKeys devices.

Configuration explanation video [Link](https://www.youtube.com/watch?v=qxPZVYqWExU).

Download [Link](https://www.poscope.com/downloads/).

### ▪ Mach3 : CNC Machine Controller Software

Mach3 turns a typical computer into a CNC machine controller. It is very rich in features and provides a great value to those needing a CNC control package.

Configuration explanation video [Link](https://www.youtube.com/watch?v=e5MjEEe-gE4&t=58s).

Download [Link](https://www.machsupport.com/downloads-updates/).

 

# Machine Building Workshop

The Machine Building Workshop was a great experience to all of us, and it was the first step to sharing knowledge with everybody.

This is a set of photos describing the general atmosphere in which passed this wonderful workshop.

## **▪ Day 1** 
**Ice breaking & debriefing around CNC machines and their purposes**
<img src="img/image028.jpg" alt="img" style="zoom:33%;" /> <img src="img/image030.jpg" alt="img" style="zoom:33%;" />

## ▪ Day 2 
Knowing everything about the design of the **CARVER X5** and the different steps will do during the workshop

<img src="img/image032.jpg" alt="img" style="zoom:33%;" /> <img src="img/image034.jpg" alt="img" style="zoom:33%;" />

## ▪ Day 3 

**-Workbench and space preparation** 

<img src="img/image036.jpg" alt="img" style="zoom:33%;" /> <img src="img/image038.jpg" alt="img" style="zoom:33%;" />

**-Frame assembly**

<img src="img/image040.jpg" alt="img" style="zoom:33%;" /> <img src="img/image042.jpg" alt="img" style="zoom:33%;" />

<img src="img/image044.jpg" alt="img" style="zoom:33%;" /> <img src="img/image046.jpg" alt="img" style="zoom:33%;" /> 

<img src="img/image048.jpg" alt="img" style="zoom:33%;" />  <img src="img/image050.jpg" alt="img" style="zoom:33%;" /> 

**-Electronic circuit schematic design**

<img src="img/image052.jpg" alt="img" style="zoom:33%;" /> <img src="img/image054.jpg" alt="img" style="zoom:33%;" />

## **▪ Day 4 & 5**
**-Y2X Bridge Assembling**

<img src="img/image056.jpg" alt="img" style="zoom:33%;" />  <img src="img/image058.jpg" alt="img" style="zoom:33%;" />

<img src="img/image060.jpg" alt="img" style="zoom:45%;" /> <img src="img/image062.jpg" alt="img" style="zoom:45%;" />

<img src="img/image064.jpg" alt="img" style="zoom:33%;" /> <img src="img/image066.jpg" alt="img" style="zoom:33%;" />

<img src="img/image068.jpg" alt="img" style="zoom:33%;" /> <img src="img/image070.jpg" alt="img" style="zoom:33%;" />

**-X2Z Assembling**

<img src="img/image072.jpg" alt="img" style="zoom:33%;" /> <img src="img/image074.jpg" alt="img" style="zoom:33%;" />

<img src="img/image076.jpg" alt="img" style="zoom:33%;" /> <img src="img/image078.jpg" alt="img" style="zoom:33%;" />

**-Electronic enclosure Assembling**

<img src="img/image080.jpg" alt="img" style="zoom:33%;" /> <img src="img/image086.jpg" alt="img" style="zoom:33%;" />

<img src="img/image082.jpg" alt="img" style="zoom:33%;" /> <img src="img/image084.jpg" alt="img" style="zoom:33%;" />

## ▪ Day 6 
**-Z-Axis assembling**

**-Plexiglas enclosure assembling** 

<img src="img/image088.jpg" alt="img" style="zoom:33%;" /> <img src="img/image090.jpg" alt="img" style="zoom:33%;" />

<img src="img/image092.jpg" alt="img" style="zoom:33%;" /> <img src="img/image094.jpg" alt="img" style="zoom:33%;" />

**-Wiring electronic parts**

<img src="img/image096.jpg" alt="img" style="zoom:33%;" /> <img src="img/image098.jpg" alt="img" style="zoom:33%;" />

 <img src="img/image0100.jpg" alt="img" style="zoom:33%;" />


## ▪ Day 7 
**Presenting the machine and Workshop roll up**

# Credits

Everything has to end, and so did the **Open Source 5 Axis CNC Building Workshop**!
This workshop passed in an amazing way, and was a great success for all of MakerLab's team!
The knowledge of one month of machine design, followed by two months of fabrication and assembly, shared with amazing people from all over Tunisia, gathered in FabLab ENIT seeking one unique goal: Learn how to construct Machines! And today, this same knowledge is being shared with the whole DIY & Open Source Hardware community.

## Partners in the Workshop
This project was launched by Open Lab Hamburg from Helmut Schmidt University, sponsored by BMBF, which we thank a lot for their confidence and the opportunity they gave to us as a startup.
This Workshop was hosted by **[FabLab ENIT](https://www.facebook.com/FabLabENIT/)**, and was successful thanks to the devotion of the participants who are from now on **"Machines Makers"**.

## Amazing people around us
We would like to thank all the **FabLab ENIT Team**, **4C Center**, **ENIT administrative staff** for their collaboration. 
Coaches **Danielli Ingressia**,  **Hashim Al SAKKAF** and **Kais ALILA**, three great Makers from the Open Source community that we had the opportunity to work and exchange ideas with.
All the gratitude and thanks to **Babasile Daniel**, for his support and encouragement. 
Special thanks too to our families and friends who supported us in this big challenge (Marouen FAKHFAKH and Rabie TAHRI)

## Makers who worked on this machine
**CARVER X5 Designers**
     -Anis TRIGUI - Project Manager, Machine Designer and Coach - CEO of MakerLab
     -Mohamed MAATOUG - Designer and Pedagogic Certified Coach - MakerLab member
**Makers of MakerLab**
Azer KHALED, Alaa MEJRI, Khalil SLAMA, Salem MBAREK, Amine MAHDHI, Jawher MANSOUR, Moez KAZDAGHLI, Yassine CHEOUR
**Machine Building Workshop Participants ( Green Team)**
Sinda BESROUR, Eya CHROUDI, Sahar FRIKHA, Mootaz BEN ZINOUBA, Hassen ARBI, Haythem LTIFI, Abderrahmen MELLITI, Youssef SAFER, Seifallah BOUCHOUCHA, Taha ISSAOUI.

## Technical Partners
And finally, we would like to thank our partners, without their help, we couldn't reach this milestone:  
- **[Fabrica-Numeric](https://www.facebook.com/Fabrica.numeric/)**
- **[ElFabSpace](https://www.facebook.com/elfabspace/)**
- **[Electronic Shop](http://electronic-shop.biz/)**

Stay tuned to learn about our new coming Open Source Machine that we are planning to construct.



# Contact

- **contact@makerlab.tn**
- **[Linkedin](https://www.linkedin.com/in/kais-alila-3a1b35163/)**
- **[Facebook](https://www.facebook.com/tunmakerlab/)**
- **[WebSite](https://www.makerlab.tn)**

# Acknowledgements

The development of this machine has been funded by:<br>
**[German Federal Ministry of Education and Research](https://www.bmbf.de/en/index.html)**

Funds implemented by:<br>
**[OpenLab Hamburg](http://openlab-hamburg.de/startpage/)**<br>
[Helmut-Schmidt-Universität Universität der Bundeswehr](https://www.hsu-hh.de/en/)<br>
Laboratorium Fertigungstechnik<br>
Holstenhofweg 85<br>
22043 Hamburg<br>

# License

<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Licence Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />Ce(tte) œuvre est mise à disposition selon les termes de la <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Licence Creative Commons Attribution 4.0 International</a>.

# Note
This documentation will be continuously improved as soon there are updates and/or improvements on the machine.

# CARVER_X5
