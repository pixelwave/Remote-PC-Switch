# remote-pc-switch
Remote PC Switch

I am currently trying to realize the following project:

I have a server rack with a number of computers (gaming, work, ..). Each computer has two monitor outs (Displayport 1.4, 4K@144Hz) and a single peripheral out (USB-C 10Gbps). 

Important bandwith parameters:
- Displayport: min. **1.4 4K@144Hz via DSC**, ideal: 2.1 4K@240Hz
- USB-C: min. **5Gbps** / ideal 10Gbps

Now I want to make those computers available at various locations (2-3). Distance varies between 10 - 30+ meters.

~~There are already a number of fiber optic solutions out there to solve the distance issue (https://fibercommand.com, https://www.heyoptics.net/) and I could basically have one of those multi cables to each terminal location:~~

~~**MPO Fiber Connection**~~
<img width="1151" alt="image" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/5a5c180c-fc97-4453-bf09-654362d0de5e">

**Both potential fibercommand and heyoptics solutions and especially customer support have proven "complicated". Will switch to a different route for now with single fiber cable solutions for DP and USB. Will update soon after cable compatibility tests.**


What is missing now is basically a switching unit in my server rack that allows me to say ComputerXYZ passthrough to TerminalXYZ.

Since are no 4K@144Hz units available I decided to built a switch myself.

This project will be periodically updated until completion!

**Updates**


**2024-04-20**

Printed case and assembled, wired up to new GIGABYTE AORUS FO32U2P (DP2.1 OLED!) monitor for further testing. Trying to find a compatible fibre DP cable that works long distance with 4K@240Hz (15M):
![IMG_3097](https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/ddf7a283-fd2a-41b6-9312-6b4dc10342ec)


**2024-04-03**

Wiring scheme and test setup complete. All assembly parts printed. Now to final testing:

![IMG_2968](https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/e4984c09-5248-4d1c-a799-0e14be96d140)
<img width="1678" alt="Screenshot 2024-04-03 at 07 58 05" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/93d60018-cd4a-4a78-ab48-1e2c54afae33">

**2024-03-03**

USB-C 2x1 switch testing finalized. Updated wiring for 4x PC inputs to 2x Terminal outputs:

![wiring](https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/5d6eeed4-9dbc-4c59-a7c0-d52c93b4a293)


**2024-02-02**

Found a good way to internally connect both splitters without producing much cable-length-waste (flat ribbon extension cables):

<img width="1006" alt="Screenshot 2024-02-02 at 15 55 30" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/cca0eb70-39d8-4c6e-82bb-556b54c42b4c">

**2024-02-01**

Just a quick update. 1U rack mount design is on-going and in current prototyping phase:

<img width="1228" alt="Screenshot 2024-02-01 at 09 33 20" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/4de433f8-9092-4467-8cbd-eb466006e6fd">

**2024-01-21**

Updated and simplified the ESP32 control scheme. Only 2 Optocouplers and 2 Controls PINs required now.

<img width="1179" alt="Screenshot 2024-01-22 at 12 03 27" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/e428fb1a-c30e-4189-b233-f0e1b8d4c131">

**2024-01-21**

Complete wireing finalized and optical equipment assembled:

<img width="944" alt="Screenshot 2024-01-21 at 12 51 43" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/79a1bded-2a69-4a56-a65c-0c4b128abae0">
<img width="1757" alt="Screenshot 2024-01-21 at 12 53 29" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/fadeb416-dd41-4f8c-a9c6-73c30b8753ff">

**2024-01-18**

Extended the diagram to support "Matrix" capability. Before only one terminal could be used simoultaneously. Now both can be used at the same time (A -> B, B -> A or A -> A, B -> B).  

<img width="1094" alt="image" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/7d6e0627-242f-4d0f-b22a-03c628b9888e">

**2024-01-16**

Hooked up DP2.1 switch to ESP32. Switching and read-out of current active port successful!

![IMG_2452](https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/03c9a8f5-4703-4f7c-8fbb-572b3ba67629)
![IMG_2453](https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/04b804be-d4b4-4ec2-a913-a52113f5b9a7)
![IMG_2456](https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/7afe72db-d579-4003-bdd6-86fe7adf5c82)

**2024-01-13**

Disassembled a low cost DP2.1 (2x1) switch and established wireing diagram:

![IMG_2437](https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/166a4d40-186a-4291-9b7a-3f8098a76c33)


**2024-01-12**

Purchased test components. Works with two DP2.1 2x1 switches in a row as intended:

![IMG_2423](https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/e069e56e-ae02-4bf7-b1aa-4f58e68b3c98)

**2024-01-10**

Established initial schematic:

<img width="1206" alt="Screenshot 2024-01-16 at 14 21 27" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/8dd494a7-66f0-4983-b391-3d5b4106e9e3">
