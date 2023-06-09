## Introduction

The purpose of the agent-based traffic simulation is to provide an access for clients to easy simulate traffic in a provided piece of road.

The traffic that will be simulated will contain one or more vehicles.

The vehicles shall have a provided speed and will be driving in a single way road. 

The end users that the system is aimed for is for any client that want to simulate a road traffic. 


## User requirements

**1.** The traffic simulation will generate a visualisation of the traffic (vehicles) on the road and also output the data/statistics of the said traffic. An interface will also be provided that will give the user the possibility of providing custom parameters for number of vehicles in traffic, max speed of vehicles, delay probability, length of road.



## System requirements

**1.01.** The simulation shall be using the agent-based computional model.

**1.02.** An agent shall have following rules:

- Acceleration: $v_{i} \Leftarrow min(v_{i},v_{max})$
- Deceleration to avoid accidents: $v_{i} \Leftarrow min(v_i,gap)$
- Randomisation: with certain probability $p$ do $v_{i}\Leftarrow max(v_{i}-1,0)$ 
- Movement: $x_{i}\Leftarrow x_{i}+v_{i}$ 
			
**1.03.** An agent is a vehicle.

**1.04.** Vehicle shall have following parameters, *Velocity*, *Acceleration*, *Deceleration*,  *Position*

**1.05.** There will be at-least three different components in the program, *simulation component*, *UI component* and *data-collection component*.

**1.06.** Simulation and UI shall run on different threads. 

**1.07.** A graphical module will output a visualisation of the traffic to the UI. 

**1.08.** The data-collection component will output an CSV file with collected data when software has runned successfully to its end. 

**1.09.** MVC architecture style will be used.

**1.10.** Java programming language will be used to to develop the simulator.

**1.11** The IDE for development of simulator will be IntelliJ

## System Overview
