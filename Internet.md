# Internet

## What is the Internet?

The Internet is a computer network that interconnects several devices such as PCs, mobiles, servers, sensors, etc. All these devices are termed as **hosts** or **end systems**. These end systems are interconnected by communication links and packet switches.

**Communication Links:** They are wired or wireless methods used to interconnect the various end systems over a network. Such communication is facilitated by the use of different types of physical media, such as copper wires, coaxial cables, optical fibres, etc. Depending on the type of physical media used, the transmission rate of information, measured in bits per second, varies. A bunch or packages of information that are transmitted over a network are called a **packets**.

**Packet switches:** They take in the packets of information coming from end systems and forward them to their destination through suitable communication links. A **router** is an example of a packet switch, which performs traffic directing functions by forwarding packets within a network.

The path taken by a packet in order to go from one end system to its destination through a number of packet switches and communication links is known as a **route**.

### API

The Internet also serves as an infrastructure that provides services to applications running on end systems. In order to achieve interoperability, the applications running on end systems connected to the Internet provide an **Application Programming Interface (API)**. The API provides a set of protocols that the transmitting end system must follow so that data can be sent to the destination end system seamlessly over the Internet.

## Who is an ISP?

The end systems are just devices located at the ends of a network. But how do they connect with other devices in the network, i.e., how do they access the Internet? This is where an ISP comes in.

**Internet Service Providers** (ISPs) allow end systems to access the Internet. Each ISP itself is a network of packet switches and communication links, and the various ISPs are in turn interconnected. We will take a closer look at this in the "Structure of the Network" section. ISPs provide various modes of internet access to the end systems, depending on various factors, which we will see in the next section.

## Routers vs Switches vs Access Points

**Modem:**
It processes the analog signals coming from the ISP through a communication link, translates it into digital signals, and interfaces it with your own home network. It also takes in the digital signals coming from an end system in your home network, coverts them into analog signals for transmission to the ISP, and in this way, connects you to the Internet.
Modem is connected to your end system using the ethernet port. If you are connecting just one wired device to the Internet, then a modem is all you need.

**Router:**
If you wish to get a host of devices in your home network connected to the Internet, such as PCs, mobile phones, gaming consoles, etc., a router is what you would need. Routers help create your own local network, with each device connected to it assigned a unique local IP address. This makes sure web traffic is navigated to the appropriate device within your network.

**Switch:**
If you have a lot of wired devices and the ethernet ports on a router aren't sufficient, then an additional network Switch can be used. They provide multiple outputs, thereby turning one ethernet port into many. They need to be connected to a router for assigning local IP addresses to each end system.

**Access Point:**
An access point is a wireless network device that is used for extending the wireless coverage of an existing network and for increasing the number of users that can connect to it.
A high-speed Ethernet cable runs from a router to an access point, which transforms the wired signal into a wireless one. Wireless connectivity is typically the only available option for access points - establishing links with end systems using Wi-Fi.

> The piece of equipment that communicates with your devices wirelessly (such as Wi-Fi routers) aren't just routers. They are a combination of **routers**, **switches**, and **wireless Access Points** (with sometimes a **modem** as well).

## Access Networks

End systems connect to the Internet by communication links, which is provided by the ISP and depends on a number of factors such as cost, location, range, speed, etc. They can be of the following types:

### 1\. Digital Subscriber Line (DSL)

DSL Internet access is provided by the local telephone company (telco), which also provides local wired phone access. Thus the local telco acts as the ISP.
It is cheaper and is used for short ranges.
Transmission rate: 1Mbps - 10Mbps

#### Role of DSL Modem:

The DSL modem, connected to the end system, uses the telephone line to connect to the Internet. It takes in the digital signals coming from the end system and translates them into analog signals to be transmitted to the DSLAM.

#### Role of DSLAM:

The analog signals transmitted through the telephone cables reach the Central Office (CO), in which the Digital Subscriber Line Access Multiplexer (DSLAM) converts it back into digital signals and sends it over the Internet.

#### Frequency bands:

Data through the telephone cables is transmitted in different frequency ranges, as shown below:

1.  Downstream channel: 50kHz - 1MHz
2.  Upstream channel: 4kHz - 50kHz
3.  Telephone channel (2-way): 0 - 4kHz

Since most people download more content than they upload, ISPs typically assign a higher frequency band for downstream channels rather than upstream. Due to this, DSL is also referred to as **ADSL** \- Asymmetric Digital Subscriber Line. If you need more upstream bandwidth, say you're running a video production company, you can get Symmetric DSL (SDSL).

At the customer's end, a splitter is used to separate the telephone channel and the Internet access channels. Similarly, the DSLAM at the CO separates the telephone channel and Internet channels, and sends the data to the Internet.

**Your connection to the ISP is your own!** Bandwidth on an incoming cable line, compared to DSL, is shared by many houses in a neighbourhood.

Also, you don't necessarily need a phone service to use DSL. Many ISPs provide DSL over a "dry-loop".

#### Drawbacks:

The farther you are located from the ISP, the slower your DSL connection will be. The residence needs to be located within 8 - 16 km of the Central Office.


### 2\. Cable

Cable Internet access is provided by the local television company, which also provides local television access. Hence the local television company acts as the ISP.
Transmission rate: 5Mbps - 50Mbps

#### Role of Cable Head end:

The Cable Head End serves a similar purpose as the Central Office (CO) in case of DSL. Fiber optics are used to connect the cable head end to neighbourhood-level junctions, from which coaxial cables are used to connect to individual homes. Since two types of cables are employed, the system is usually called Hybrid Fiber Coax (HFC).

#### Role of Cable Modem:

Just like a DSL Modem, the Cable modem too connects to the end system and uses television cables for Internet access. It takes in the digital signals coming from the end system and translates them into analog signals to be transmitted to the CMTS.

#### Role of CMTS:

The Cable Modem Termination System (CMTS) serves a purpose similar to the DSLAM. It takes in the analog signals transmitted through the television cables from the cable modems, converts the signals back to digital and sends them over the Internet.

#### Drawbacks:

Packets of data exchanged between the end systems and the CMTS flow through every home. Due to this, if several users are downloading a video, then the speed would be significantly lower than the normal downstream transmission rate.


### 3\. Fiber to the Home (FTTH)

Reference - https://searchnetworking.techtarget.com/definition/fiber-to-the-home

Fiber to the Home (FTTH) is the use of optical fibers from the Central Office to residences to provide Internet access, thereby replacing existing copper infrastructure such as telephone wires and coaxial cable. FTTH dramatically increases Internet speeds compared to previously discussed network access methods.
Transmission rate: 250Mbps - 1000Mbps. This is about 20-100 times faster than DSL and Cable Internet access methods.


> ### DSL vs Cable vs Fiber
> 
> https://broadbandnow.com/guides/dsl-vs-cable-vs-fiber

### 4\. Ethernet

Ethernet is a communication standard used to network computers and other devices in a LAN. It is defined in the IEEE 802.3 standard.
Transmission rate: Supports bandwidths between 1Mbps - 100Gbps.

It is a wired system that started with using coaxial cable and has now evolved to using twisted pair wiring and fiber optical cables.

#### CSMA/CD:

Ethernet transmits data using an algorithm called CSMA/CD, which stands for **Carrier Sense Multiple Access with Collision Detection**, to reduce data collisions and improve successful data transmission. The algorithm first checks whether there is any traffic on the network. If it does not find any, it will send out the first bit of data to see if any collision will occur. If the first bit is successful, it will send out the other bits while still testing for collisions. If a collision occurs, the algorithm calculates a waiting time and then starts the process again until the entire data exchange process is complete.

> #### Additional Info
> 
> RJ45 - https://youtu.be/sbXe__EtGg4

### 5\. Wi-Fi

Wi-Fi is a wireless technology that uses radio signals to connect various devices over a local network and provides Internet access.
It allows users to wirelessly transmit/receive packets of data to/from an access point. This access point (usually present inside a router) is in turn connected to the Internet using wires. Thus, the access point/router acts as a hub to broadcast the Internet signals to all your Wi-Fi enabled devices.

#### Hotspot:

A hotspot is an actual location in which people can access the Internet using their devices such as laptops, tablets, mobile phones, etc.
Hotspots can be either public or private. Examples of public hotspot - hotels, airports, cafe, etc. Private hotspots could be your home.

Hotspots are created using a Wi-Fi router or an access point, which is connected to the ISP and provides Internet access to the devices connected in the hotspot.

**Tethering:** This is a method of creating a private hotspot using your smartphone. Smartphones get their Internet access using cellular networks and you can transform your smartphone into a wireless access point, allowing you to connect other devices to the Internet.

**Mobile Hotspot:** It is a portable device that uses cellular networks for Internet access, and allows you to connect other devices to the Internet.

> ### Ethernet vs Wi-Fi
> 
> **Why is Ethernet always faster than Wi-Fi?**
> Although EM waves move faster in air than electrons move through a wire, ethernet internet access is always faster than Wi-Fi, no matter how much money you spend wireless gear. This is because of the following reasons:
> 
> 1.  Signal deterioration: Radio signals flying through the air such as Wi-Fi signals are more susceptible to noise than in case of ethernet, resulting in signal degradation. Ethernet cables are shielded from external waves to prevent interference, and hence can travel longer distances. Wi-Fi signals would have to compete with other Wi-Fi signals, microwave signals, walls, etc.
> 2.  More latency: Ethernet uses CSMA/CD algorithm to prevent collisions by sending packets of data immediately after the channel is free. Wi-Fi, on the other hand, introduces a small delay once the channel becomes clear. Since Wi-Fi routers cannot detect collisions mid-air, this delay reduces the risk of collisions, but at the same time, adds more latency.
> 3.  Old communication protocol: Wi-Fi is half-duplex, which means that the Wi-Fi router's antenna can only send or receive packets of data at a time, but cannot do both simultaneously. Ethernet on the other hand, is full-duplex, i.e., it can send and receive data simultaneously, as an ethernet cable contains two wires - one for receiving data and the other to transmit data.

## Structure of the Network (Network of Networks)

## Protocols

## Traceroute

> ## Additional Info
> 
> https://youtu.be/kx3qwqtZvs4
