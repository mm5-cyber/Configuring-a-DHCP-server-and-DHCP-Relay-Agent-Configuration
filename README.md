# Cisco Packet Tracer: Fundamentals & Configuring-a-DHCP-Server-and-DHCP-Relay-Agent-Configuration


## Objective

To learn Networking Fundamentals using Cisco Packet Tracer, and using my knowledge gained from educational videos to create a networking scenario that I can effectively troubleshoot and fix. 

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

Using this resource, these are the projects that I followed: 

1.  Navigating the Interface & Adding / Removing Modules on a device

 <img width="731" height="556" alt="image" src="https://github.com/user-attachments/assets/7bb799c7-75d3-4c53-924f-d18d8b15d931" />

 <img width="357" height="442" alt="image" src="https://github.com/user-attachments/assets/262f630f-cd07-48f4-980b-fcee8285ebed" />


2. Creating a connection between two computers through the use of Copper Cross-over Cables connectied via each computers fast ethernet port (fa0). 

  <img width="325" height="109" alt="image" src="https://github.com/user-attachments/assets/e7fe46dc-df8c-43be-aa1d-5aafa6e0b6a4" />

  To actually enable the communication, each computer was assigned with a seperate static IP addres within their IP Configuration section, on the simulated Desktop tab.

  <img width="715" height="250" alt="image" src="https://github.com/user-attachments/assets/bedba3c0-92ad-441b-8f9d-b7470c7c271b" />

  <img width="905" height="440" alt="image" src="https://github.com/user-attachments/assets/197873ad-2ceb-41c2-8fe7-6d70db06b313" />

3.  Simulate a "Star Topology Network" by connecting end devices to a common switch via Copper Straight-Through cabling.

  <img width="354" height="240" alt="image" src="https://github.com/user-attachments/assets/f3569994-b90a-4ee5-b715-0cb076bae997" />


4.  Connecting two switches together using Copper Cross-over cables.

  <img width="940" height="372" alt="image" src="https://github.com/user-attachments/assets/519f5f99-5a47-4c82-a01d-df1a2e21dbde" />

  Using the Physical Tab, I situated the two switches and their associated end-devices into seperate "Wiring Closets", situated within the same building

  <img width="940" height="492" alt="image" src="https://github.com/user-attachments/assets/5c9ba595-1f84-4243-bea1-11ef20518e39" />

  <img width="419" height="694" alt="image" src="https://github.com/user-attachments/assets/2b023260-7362-466b-abc1-c628d18313b9" />


5. Seperating switches and their respected devices into seperate subnets, these of which can then only be communicated with through a router.

   <img width="940" height="546" alt="image" src="https://github.com/user-attachments/assets/5686a9a3-8806-411c-bc91-41239fc3a066" />

 The switches connect to the Cisco 1941 router via copper straight-through cables into the router’s Gigabit Ethernet ports. The router used only has two Gigabit Ethernet ports, which is fine for this prac. 
 
The devices connected to Switch 1 (left side of the diagram) fall under the IP address range of 192.168.1.x, and their default gateway is 192.168.1.1 The devices of switch two (right side of the diagram) are set to 172.16.1.x, with their default gateways being set to 172.16.1.1.

In the router, I configured the default gateway of Gig 0/0 to 192.168.1.1, and for Gig 0/1, I used 172.16.1.1.
Within the router’s config setting for the Gigabit Ethernet connections. The “Port Status” setting had to be checked. This is pretty much the power-on button for the connections. 

Now the connections are established for each end device to successfully communicate with the other, even if they are situated in seperate subnets. This couldn’t be done through switch connection alone, and it helped me understand the importance of routers in network architecture.


6. Connect devices wirelessly through an "Access Point"
 
<img width="666" height="436" alt="image" src="https://github.com/user-attachments/assets/9f6387e3-2a9f-43af-9d1e-9b3e4ef3b57e" />  

To have devices connect to an access point wirelessly, the access point's "Port 1" had to be configured with an SSID (Service Set Identifier), Authentication Method (WPA2-PSK), and PSK (Pre-shared Key) Passphrase. This allows other devices to be able to find and connect to the access point through configuring their wireless networks. 

However, the devices on their own (except the tablet) by default, were only able to connect to other devices through Ethernet. Therefore, I had to power off the devices and replace their Ethernet modules for a "WPC300N Adapter". The devices were then turned back on.  

<img width="563" height="446" alt="image" src="https://github.com/user-attachments/assets/fbb3a147-45b8-4f02-a3ea-434d120be5a9" />  

The devices were then able to connect to the Access Point through the "PC Wireless" section of their "Desktop Tab", simply through searching for the available network connection, and typing in the PSK. 


<img width="562" height="460" alt="image" src="https://github.com/user-attachments/assets/302b2cd8-9493-4f37-8bda-aac4f6f2e14c" /> 

However the signal of the connection is very weak, sitting at only 39%. That is when I switched from logical to physical mode, to place all of the devices into the same wiring closet, resulting in a signal strength of 100%. This demonstrates that Cisco Packet tracer takes into consideration the physical distance between each device. 

<img width="1084" height="691" alt="image" src="https://github.com/user-attachments/assets/a8c3d821-ecea-4233-b95c-d3d70cfa1f67" />


<img width="355" height="264" alt="image" src="https://github.com/user-attachments/assets/a401d22a-6fcd-46fd-9f72-bf772c68cd59" /> 

7. Configuring a DHCP & Mail Server



I connected a server to a simple Star Topology network. However, instead of manually assigning static IP's to each end device, I wanted to make the server automatically assign IP addresses through the Dynamic Host Protocol (DHCP) Service. By configuring the service as shown below, I was able to assign the IP address range of 192.168.1.10-20 to all end devices in the network. However, I did have to assign a static ip address of 102.168.1.9 to the server, to allow connectivity to happen. 

<img width="1290" height="667" alt="image" src="https://github.com/user-attachments/assets/ea1d774c-2847-4cb3-9a51-ce20109b1e3e" />

As long as each end device has their IP configuration set to DHCP, and they are in the same network, they would automatically recieve an IP address within the specific range that server pool has been configured to. 

<img width="539" height="98" alt="image" src="https://github.com/user-attachments/assets/356b093f-14b0-46ce-80a4-aa4992d4ee8b" /> 

Using the same network topology, I configured the server to allow email services. I added two users under the server's email service tab, falling under the domain of gmail.com. 


<img width="1318" height="567" alt="image" src="https://github.com/user-attachments/assets/adbd7e4c-a595-4585-8769-4556f585d013" /> 

Then on the respective end devices, I plugged in the same email and login names into their email configuration settings section. 


<img width="1338" height="666" alt="image" src="https://github.com/user-attachments/assets/17a996e4-a9eb-49f3-b094-83d2867a2ac9" /> 

I tested the connectivity by sending a message from "Mike's PC" to "Mitch's PC" 


<img width="1379" height="670" alt="image" src="https://github.com/user-attachments/assets/ad0ec580-1d70-46d7-9641-cd2865fdf076" />

If the username, login, and domains didn't match to the email server, than the message wouldn't be able to transmit from one computer to another. 



## Personal Project 

My personal project was heavily influences by projects 5. and 7. The main goal is to have end devices recieve their IP's on a DHCP server that is located on a completely seperate subnet. The only way that they could connect is through a router. I thought this project would be fairly straight-forward but I came across an issue in which I had to troubleshoot on my own.

This is what the network topology of this project lookls like:  

<img width="1056" height="486" alt="image" src="https://github.com/user-attachments/assets/07705625-f414-45e4-b192-944fe325f960" /> 

The left side of the router is the 192.168.1.x subnet, and the right side is the 172.16.1.x subnet. 

The server is located on the 172.16.1.x subnet. 

The server has two DHCP server pool configurations.  

<img width="1084" height="753" alt="image" src="https://github.com/user-attachments/assets/7313bb3b-aabe-4704-8bf0-5e2667417338" />

This one is for all the devices in the 192.168.1.x subnet. 

<img width="1078" height="762" alt="image" src="https://github.com/user-attachments/assets/db0e8981-29d2-45b2-aa8b-019047c9b766" />

This one is for all the devices in the 172.16.1.x subnet.  

Each end device's IP Configurations are set to "DHCP" not "Static". This means that the end devices are waiting for the DHCP server to assign them their IP's. 

The only devices with a static IP configuration are the router, and the Server itself. 

The router's Gigabit Ethernet 0/0 Port is set to 192.168.1.1, and Gigbit Ethernet 0/1 is set to 172.16.1.1. Gig0/0 is the default gateway for the devices on the 192.168.1.x suvnet, and Gig0/1 is the default gateway for the devices on the 172.16.1.x subnet. 

The server's static IP is set to 172.16.1.9, which is outside of the range of IP addresses it provides to the end devices. It's default gateway also has to be manually configured via static IP. This is so that clients can consistently find them without network disruptions. 

## The problem

The main issue with this network, is that the DHCP server cannot assign the IP addresses to the end devices on the other subnet. As you can see from this example below, the DHCP server has successfully assigned PC2 with the IP address of 172.16.1.10. In a seperate tab the default gateway has also been set to 172.16.1.1, which is what is intended happen. 

<img width="2074" height="578" alt="image" src="https://github.com/user-attachments/assets/6647dcbe-0e5c-4aac-a3ee-2c9fd0fa32cc" />

However, let's take a look at PC1, which is located on the opposite subnet.  

<img width="2182" height="637" alt="image" src="https://github.com/user-attachments/assets/5dab6ddc-6d0f-4385-8331-52002640e003" /> 

<img width="2237" height="615" alt="image" src="https://github.com/user-attachments/assets/329aa872-4ad7-4d39-bf5d-0734a2754596" /> 

The IP address is set to this computer is "169.254.82.235", and no default gateway is set. The IP address shown is known as an Automatic Private IP Address (APIPA). According to Lenovo, APIPA's only connect devices locally on the same subnet, and they are created only when no DHCP server is available. The APIPA typically falls into the 169.254.x.x range (Lenovo, 2026).  This is not what we want, as this clearly indicates that the DHCP server has failed to reach these devices.

So I asked to myself, why is this happening? So I did some research. 

## The Why? 

According to Martin L, a user on the Cisco Community forum, a DHCP Packet is sent out as a "broadcast", which is when a networking device is sent to every device on a local network (L M, 2023). Routers block these requests by default for security reasons, and to prevent network congestion.


## What is the fix? 

After realising that the main issue has got to do with the router not allowing DHCP traffic through, I searched up a guide on how to allow this traffic through. This is where I found out about a DHCP Relay Agent, which allows the forwarding of DHCP broadcast messages to clients situated at a different subnet. 

The video by "Network Engineer Stuff" showed me the exact router CLI commands needed to make this work (Network Engineer Stuff, 2025).

<img width="477" height="153" alt="image" src="https://github.com/user-attachments/assets/757feaee-8f65-4a12-a1bf-5af74292e119" />

The commands used: 

Router>en - enables Privileged EXEC mode, allowing the use of administrative commands. It's like sudo in Linux. 

Router#config t- configure terminal, allows changing system-wide settings of the router. 

Router(config) #int Gig0/0 - Changes into interface configuration mode for Gig0/0 (192.168.1.x subnet). This allows the use of IP helper command to enable DHCP Relay. 

Router(config-if)#ip helper-address 172.16.1.9 - It configures the DHCP Relay Agent, It allows the router to listen to the broadcast requests sent from a client, and forward them to the DHCP server on a different subnet. In the command, the IP used is the DHCP Server's static IP address. 

Router(config-if)#^Z - Returns you out of configuration mode

wr - Stands for "write memory", it saves the currently active configuration from RAM to NVRAM. Essentially ensuring that your changes are saved and applied the next time the device reboots. This means that you don't have to keep typing the commands listed above upon each startup. 


## What I learned 

I gained practical troubleshooting experience by:

- Verifying default gateway configurations.

- Ensuring DHCP pools match the correct subnet ranges.

- Confirming the server’s static IP sits outside the DHCP scope.

- Finding out that APIPA is a clear indicator of a DHCP failure 

- Testing DHCP behaviour before and after relay configuration.

Improved my understanding of: 

- Broadcast vs unicast traffic

- Router interface roles and gateway responsibilities

- DHCP pool design

- Relay agents and their role in enterprise networks

- How routing and DHCP interact in multi‑subnet environments

## Credit 

https://www.lenovo.com/us/en/glossary/what-is-apipa/ 

https://www.youtube.com/watch?v=ty0HMs48U1k&t=2056s  

https://community.cisco.com/t5/switching/packet-tracer-dhcp-server-not-assigning-ip-s-to-other-networks/td-p/4955813


















