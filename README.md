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
