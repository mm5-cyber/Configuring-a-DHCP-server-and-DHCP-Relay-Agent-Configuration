# Configuring-a-DHCP-server-and-DHCP-Relay-Agent-Configuration

## Objective

This Home Lab project aims to prevent unauthorised access to my network, to protect sensitive data. The router acts as the main gateway between the internet and your home/office devices, securing it prevents it from becoming a "front door" for attackers.The primary focus of this is to access the web server of the router, and make adjustments to its configurations to prioritie security over availability. 

### Skills learned

- Network Design Fundamentals 
- Cisco IOS CLI Command Foundations
- IP Addressing & Subnetting
- Troubleshooting: Using diagnostic commands like ping, traceroute, show ip interface brief, and show cdp neighbors to isolate connectivity issues and routing loops


### Tools used

- Cisco Packet Tracer
- Cisco IOS CLI 


## Learning Cisco Packet Tracer

<b>What is Cisco Packet Tracer?</b> 

Cisco Packet Tracer is a software used for visualising Network Topologies. It allows for users to create and configure their own networks without the need of spending money on expensive equipment. I learnt the fundamentals of this software so that I can have a comprehensive understanding of Network Architecture & Design. 

Within the Software, there are two tabs. The "Logical" and the "Physical Tab". 

The key difference between these two tabs are that the logical tab allows you to create and manage hypothetical networks simply by dragging and dropping network, and end devices; Which can then be connected together via their respected cabling. It is meant for protocol testing, routing, configuration, and packet simulation. 

The physical tab highlights a hierarchial level of physical containers. Going from Outside of Cities (Cities Connecting to Cities)  - Within Cities (Buildings connecting to buildings) - Within Buildings (Rooms connected to Rooms), and Wiring Closets within rooms. It provides a great visualisation on how physical hardware, and cabling are managed. 



## What I learned 

By following a YouTube tutorial by DigiDev on the foundations of Cisco Packet Tracer, I was able to gain a comprehensive understanding of how end devices connect with each other on different networks, how switches and routers work, and what servers allow you to do. These of which, I found difficult to grasp  by just reading documentation alone. 

Using this resource, I learnt how to:

- Navigate the Interface

 <img width="731" height="556" alt="image" src="https://github.com/user-attachments/assets/7bb799c7-75d3-4c53-924f-d18d8b15d931" />

- Add / Remove Modules on a device

  <img width="357" height="442" alt="image" src="https://github.com/user-attachments/assets/262f630f-cd07-48f4-980b-fcee8285ebed" />


- Create a connection between two computers through the use of Copper Cross-over Cables connectied via each computers fast ethernet port (fa0). 

  <img width="325" height="109" alt="image" src="https://github.com/user-attachments/assets/e7fe46dc-df8c-43be-aa1d-5aafa6e0b6a4" />

  To actually enable the communication, each computer was assigned with a seperate static IP addres within their IP Configuration section, on the simulated Desktop tab.

  <img width="715" height="250" alt="image" src="https://github.com/user-attachments/assets/bedba3c0-92ad-441b-8f9d-b7470c7c271b" />

  <img width="905" height="440" alt="image" src="https://github.com/user-attachments/assets/197873ad-2ceb-41c2-8fe7-6d70db06b313" />

- Simulate a "Star Topology Network" by connecting end devices to a common switch via Copper Straight-Through cabling.

  <img width="354" height="240" alt="image" src="https://github.com/user-attachments/assets/f3569994-b90a-4ee5-b715-0cb076bae997" />


- Connecting two switches together using Copper Cross-over cables.

  <img width="940" height="372" alt="image" src="https://github.com/user-attachments/assets/519f5f99-5a47-4c82-a01d-df1a2e21dbde" />


- Connect devices wirelessly through an "Access Point"
 
<img width="666" height="436" alt="image" src="https://github.com/user-attachments/assets/9f6387e3-2a9f-43af-9d1e-9b3e4ef3b57e" />




