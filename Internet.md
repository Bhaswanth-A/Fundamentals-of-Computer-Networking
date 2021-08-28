# Internet

## What is the Internet?

The Internet is a computer network that interconnects several devices such as PCs, mobiles, servers, sensors, etc. All these devices are termed as **hosts** or **end systems**. These end systems are interconnected by communication links and packet switches.

**Communication Links:** They are wired or wireless methods used to interconnect the various end systems over a network. Such communication is facilitated by the use of different types of physical media, such as copper wires, coaxial cables, optical fibres, etc. Depending on the type of physical media used, the transmission rate of information, measured in bits per second, varies. A bunch or packages of information that are transmitted over a network are called **packets**.

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
If you have a lot of wired devices and the ethernet ports on a router aren't sufficient, then an additional network switch can be used. They provide multiple outputs, thereby turning one ethernet port into many. They need to be connected to a router for assigning local IP addresses to each end system.

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

Since most people download more content than they upload, ISPs typically assign a higher frequency band for downstream channels rather than upstream. Due to this, DSL is also referred to as **ADSL** \- **Asymmetric Digital Subscriber Line**. If you need more upstream bandwidth, say you're running a video production company, you can get **Symmetric DSL (SDSL)** as well.

At the customer's end, a splitter is used to separate the telephone channel and the Internet access channels. Similarly, the DSLAM at the CO separates the telephone channel and Internet channels, and sends the data to the Internet.

**Your connection to the ISP is your own!** On the other hand, bandwidth on an incoming cable line, compared to DSL, is shared by many houses in a neighbourhood.

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

Hotspots can be either public or private. Examples of public hotspot - hotels, airports, cafe, etc. A private hotspot could be your home.

Hotspots are created using a Wi-Fi router or an access point, which is connected to the ISP and provides Internet access to the devices connected in the hotspot.

**Tethering:** This is a method of creating a private hotspot using your smartphone. Smartphones get their Internet access using cellular networks and you can transform your smartphone into a wireless access point, allowing you to connect other devices to the Internet.

**Mobile Hotspot:** It is a portable device that uses cellular networks for Internet access, and allows you to connect other devices to the Internet.

> ### Ethernet vs Wi-Fi
> 
> **Why is Ethernet always faster than Wi-Fi?**
> Although EM waves move faster in air than electrons move through a wire, ethernet internet access is always faster than Wi-Fi, no matter how much money you spend wireless gear. This is because of the following reasons:
> 
> 1.  Signal deterioration: Radio signals flying through the air such as Wi-Fi signals are more susceptible to noise than in case of ethernet, resulting in signal degradation. Ethernet cables are shielded from external waves to prevent interference, and hence can travel longer distances. Wi-Fi signals would have to compete with other Wi-Fi signals, microwave signals, walls, etc.
> 
> 2.  More latency: Ethernet uses CSMA/CD algorithm to prevent collisions by sending packets of data immediately after the channel is free. Wi-Fi, on the other hand, introduces a small delay once the channel becomes clear. Since Wi-Fi routers cannot detect collisions mid-air, this delay reduces the risk of collisions, but at the same time, adds more latency.
> 
> 3.  Old communication protocol: Wi-Fi is half-duplex, which means that the Wi-Fi router's antenna can only send or receive packets of data at a time, but cannot do both simultaneously. Ethernet on the other hand, is full-duplex, i.e., it can send and receive data simultaneously, as an ethernet cable contains two wires - one for receiving data and the other to transmit data.

## Structure of the Network

The network of networks that forms the Internet has evolved over the years into a complex structure. As we've seen before, end systems can connect to the local or access ISPs by different modes (discussed above). The structure of the network majorly comprises of the following:

1.  **Access ISP:** The end goal is to interconnect all these access ISPs so that every end system over the Internet can exchange data packets with each other. One way to achieve this is for aceess ISPs to directly connect with each other. Such a mesh design is too costly for the access ISPs, as it would require each access ISP to have a separate communication link to each of the thousands of other access ISPs all over the world. This is where *global transit ISPs* would come into picture.
    
2.  **Global ISP:** Global ISPs span over the globe and have at least one router near each of the thousands of access ISPs. All the access ISPs connect to one (or more) of the global ISPs, rather than connecting with each other directly. Since building such a massive network is extremely expensive for a gloabl ISP, it would charge the access ISPs connecting to it depending on the amount of traffic exchanged. These global ISPs would in turn have to connect with each other so that access ISPs connected to different global ISPs can communicate with each other.
    
3.  **Regional ISP:** It is not possible for global ISPs to connect with each and every access ISP, unless they have a very impressive global coverage. To tackle this issue, the access ISPs in a region connect to the regional ISP, which in turn connects to the global ISP.
    
4.  **Multi-homing and IXPs:** In addition to just one-to-one connectivity, access ISPs can multi-home with two or more regional ISPs, and regional ISPs can multi-home with two or more global ISPs. At every level, customer ISPs pay their provider ISPs to obtain global Internet interconnectivity. To reduce these costs that a customer ISP pays to the provider ISP, a pair of nearby ISPs at the same level of the hierarchy can peer - they can directly connect their networks together so that all the traffic between them passes over the direct connection rather than through upstream intermediaries. In such a case, neither ISP pays the other. Along these same lines, a third-party company can create an Internet Exchange Point (IXP), which is a meeting point where multiple ISPs can peer together.
    
5.  **Content providers:** In recent years, major content providers such as Google have created their own private networks. These private networks carry traffic only to/from their data centers. They peer with the access ISPs by connecting with them directly or at the IXPs. Such kind of infrastructure gives a greater control on how its services are delivered to the end users.

## Addressing

### IP Addressing

In order for end systems connected over the Internet to exchange data with each other, it is important to assign an address to each so that they can find and locate the end system requesting for data. Such an address is called the **IP (Internet Protocol)** Address.

IP Address is of two types:

1.  IPv4
2.  IPv6

#### IPv4

[Reference](https://en.wikipedia.org/wiki/IPv4)

**Internet Protocol version 4 (IPv4)** is the fourth version of the Internet Protocol (IP).

It has the format $N.N.N.N$ ($32$ bits)
where $N$ has a range from $0$ to $255$ \- 8 bits

Since the IP Address of a device needs to be unique, only a total of $2$<sup>$32$</sup> devices can be connected over the Internet.

#### IPv6

[Reference](https://en.wikipedia.org/wiki/IPv6_address#:~:text=IPv6%20addresses%20are%20classified%20by,address%20to%20that%20specific%20interface.)

**Internet Protocol Version 6 address (IPv6)** is the successor to IPv4. It was developed to deal with the problem of IPv4 exhaustion, so as to have a vastly enlarged address space.

It has the format $N:N:N:N:N:N:N:N$ ($128$ bits)
where $N$ is a hexadecimal number of the format $XXXX$

A total of $2$<sup>$128$</sup> devices can be connected over the Internet.


IP Addresses can be classified into two types:

1.  Dynamic IP Address: The IP Address of the device changes every time it connects to the Internet. This IP Address is provided by the ISP from a range of available IP Addresses.
2.  Static IP Address: The IP Address of the device is fixed.

> https://www.youtube.com/watch?v=aor29pGhlFE

### MAC Addressing

MAC Address, which stands for **Media Access Control**, is a unique identifier that is assigned to a **Network Interface Card (NIC)** by the manufacturer. They are physical addresses, unique and cannot be changed. 

The address is 48 bits long (6 bytes). The first 24 bits (or 3 bytes) is called the **Organizational Unique Identifier (OUI)** which identifies the manufacturer. IEEE Registration Authority Committee assigns these MAC prefixes to its registered vendors. The last 24 bits is a unique value that is assigned by the manufacturer. 

#### Why do we need MAC Address?
Let's say we have a lot of devices connected to a router/switch. These devices, which form a local network, are connected to the Internet. When one device requests for some information, the data is fetched and brought to the router/switch. The router/switch then navigates this information to the correct device using its MAC Address.

#### What is the difference between MAC Address and IP Address?
IP addresses are used to find and locate the end system requesting for data, and to get the data to its destination. You can think of IP Address as the address to your home - data is brought to your router.

MAC Addresses, on the other hand, is more like your name. It is unique for every device and helps your router navigate data correctly _(with the help of IP Address as well)_ when many devices are connected to it in the local network, preventing data requested by on device on reaching another device connected to the same router.

As your address will change if you travel from one place to another, the IP Address of your device will also change when you connect to a different network. However your name will not change when you travel to a different location, and in a similar manner, your MAC Address also will not change.

### Port Addressing

Let's say we want to access a particular web service. To do so, we type in the URL of the website that we want to visit. The first thing that the computer will do is convert this URL into an IP Address. The computer then sends the request to the webserver. But this server might not just be hosting a website (using HTTP), it may also host a mail server (using SMTP) or a file server (using FTP). 

To navigate the request to the correct server, port numbers are used. Each application is assigned a particular port number - HTTP is assigned port number 80, SMTP is assigned port number 25, and FTP is assigned port number 20 and 21. Since these are standard port addresses, all computers will know about them. 

On making a request to the web server, our computer adds a destination port number (DST) of 80 to the TCP header, since we are accessing a HTTP site. The computer will also choose a randomly generated source port number to receive a reply. The IP Address and the port number are sent along with the request packet. The web server will see the port number, will realize that the request is meant for the web server and passes it to that application. The server then reponds, and the IP Address and port number of the source system are sent along with the response packet. 

On receiving the response, our computer will look at the port number and sends it to the relevant application, which in our case is the browser, and displays it on the particular tab as well.  

Range of port numbers: 0 - 65535

0 - 1023 are Well known port numbers

1024 - 49151 are Registered port numbers

49152 - 65535 are Dynamically assigned port numbers

Some of the common well known port numbers are:

|Application|Protocol|Port number|
|:---:|:----:|:----:|
|FTP Data| TCP| 20|
|FTP Control| TCP| 21|
|SSH|TCP|22|
|Telnet|TCP|23|
|SMTP|TCP|25|
|DNS|TCP/UDP|53|
|DHCP|UDP|67, 68|
|TFTP|UDP|69|
|HTTP|TCP|80|
|POP3|TCP|110|
|SNMP|UDP|161|
|HTTPS|TCP|443|

## Switching methods

