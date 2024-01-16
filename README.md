# remote-pc-switch
Remote PC Switch

I am currently trying to realize the following project:

I have a server rack with a number of computers (gaming, work, ..). Each computer has two monitor outs (Displayport 1.4, 4K@144Hz) and a single peripheral out (USB-C 10Gbps). 

Important bandwith parameters:
- Displayport: min. **1.4 4K@144Hz via DSC**, ideal: 2.1 4K@240Hz
- USB-C: min. **5Gbps** / ideal 10Gbps

Now I want to make those computers available at various locations (2-3). Distance varies between 10 - 30+ meters.

There are already a number of fiber optic solutions out there to solve the distance issue (https://fibercommand.com, https://www.heyoptics.net/) and I could basically have one of those multi cables to each terminal location:

**MPO Fiber Connection**
<img width="1151" alt="image" src="https://github.com/pixelwave/Remote-PC-Switch/assets/19491804/5a5c180c-fc97-4453-bf09-654362d0de5e">


What is missing now is basically a switching unit in my server rack that allows me to say ComputerXYZ passthrough to TerminalXYZ.

Since are no 4K@144Hz units available I decided to built a switch myself.

This project will be periodically updated until completion!

**Updates**

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


