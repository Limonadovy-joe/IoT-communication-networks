# IoT Communication Networks

- [Types of IoT Networks](#types-of-iot-networks)
  - [Cellular networks](#cellular-networks)
    - [Advantages of cellular IoT](#advantages-of-cellular-iot)
    - [Types of networks cellular](#types-of-networks-cellular)
    - [Narrowband IoT](#narrowband-iot) 
    - [Long term evolution](#long-term-evolution)
    - [Devices overview](#devices-overview)
  - [LAN - PAN networks](#lan-pan-networks)
  - [LPWANs](#lpwans)
    - [Narrowband IoT](#narrowband-iot)
    - [LoRaWAN](#lorawan)
  - [Mesh network](#mesh-network)
    - [Zigbee](#zigbee)
    - [ZWawe](#zwawe)
    - [RFID](#rfid)
- [Notes](#notes)   


## Types of IoT Networks
- Several factors impact the choice of a specific IoT network. These factors include **coverage area, cost, device environment, density of IoT devices, power consumption, machine-to-machine communication requirements** <sup>[1](#notes)</sup>, **network bandwidth, and security**
- IoT networks can be classified into four main categories: cellular networks, LAN/PAN, LPWAN, and mesh protocols

### Cellular networks
- Celulární neboli buňková rádiová síť 
- A cellular network or mobile network is a telecommunications network where the link to and from end nodes is wireless and the network is distributed over land areas called **cells**. Each served by at least one fixed-location **transceiver** <sup>[2](#notes)</sup>
- The most common example of a cellular network is a **mobile phone (cell phone) network**. A mobile phone is a portable telephone which receives or makes calls through a **cell site (base station) or transmitting tower**. Radio waves are used to transfer signals to and from the cell phone.
- While cellular networks were designed for phones, they’re highly versatile, cellular IoT devices can use **2G - GSM standart, 3G - UMTS standart, 4G - LTE, LTE Advanced,WiMAX , and 5G networks.**
- Specialized cellular networks have also been developed specifically for IoT: **LTE-M and NB-IoT.**

#### Advantages of cellular IoT
- **Global coverage**
  - For large-scale global deployments, **cellular M2M connectivity** is generally considered the most reliable and beneficial connectivity method.
  - As you deploy in new countries, your **cellular provider** may have roaming agreements with another carrier that covers that region. **Using global IoT SIM cards**, you don’t need to install new SIM cards, create new SKUs, or start new contracts to change your devices’ coverage.
  - Cellular is a **WAN (wide area network)** with the long-range ability to connect globally using radio waves, which are sent and received via cell towers.
  -  WiFi connectivity requires your device to remain much closer to the access point/router. Bluetooth connectivity is also short range, requiring your device to be within 10–100 meters of the access point
- **Built-in authentication**
  - Cellular networks use **SIM cards to authenticate devices**, associate them with a legitimate subscriber, and provide secure connectivity.
  - Hackers can spoof IP addresses, but they can’t spoof a subscriber’s identity, **which is stored on a SIM card.**
 
  #### Types of networks cellular
- More complex networks also tend to have more expensive modems. Generally speaking, the more advanced a network is, the more power connected devices will consume while in **“idle mode"**.
- 2G networks will soon be a thing of the past. 3G is on its way out the door, too.
- 4G LTE networks: For more complex IoT solutions. 5G networks: The future of IoT- 5G networks don’t have very widespread coverage yet.
- **Low power wide area networks (LPWAN)**
  - LPWANs allow IoT devices to **transmit or receive updates at fixed intervals or in response to an external trigger (such as a sensor)**, **rather than maintaining a continuous connection.** This drastically decreases power consumption.
  - There are two main types of LPWANs: **NB-IoT and LTE-M.**

#### Narrowband IoT
- NB-IoT
- APN stands for **Access Point Name.** It's a configuration setting used by cellular networks to connect a mobile device to a **specific gateway <sup>[3](#notes)</sup> between the carrier's network and the internet or another external network**
- Narrowband-IoT takes advantage of **gaps in the radio frequency spectrum** to provide more efficient connectivity and **prevent interference**. These unused frequency bands are known as **“guard bands.”**
- While **cellular networks like 4G LTE use broadband connections** (which support a wide range of radio frequencies), narrowband connections isolate devices to “narrower” ranges.
- Narrowband-IoT introduces two major power-saving features: **power saving mode (PSM) and discontinuous reception (DRX)**. PSM essentially puts the device to sleep when not in use, and **DRX can extend the period that the device isn’t “actively listening” for a signal.**  

#### Long term evolution
- Long term evolution **(LTE-M)**
-  Is an offshoot of LTE technology specifically designed for the Internet of Things.
-  It lets IoT devices connect to 4G networks, **giving them more bandwidth and mobility than NB-IoT**, as well as access to voice over long term evolution **(VoLTE)** — a more advanced voice service.
- Despite the greater power usage, LTE-M can still leverage PSM and DRX to significantly extend a device’s battery life
- When a device needs to transmit or receive a larger volume of data, **LTE-M uses less power than NB-IoT because the higher bandwidth allows it to upload and download data significantly faster.**



#### Devices overview
- microcontrollers with integrated nb-iot modul
  - LilyGO TTGO T-SIM7000G ESP32-WROVER-B 18560 Solar
    - [Product](https://pt.aliexpress.com/item/4000542688096.html)
    - [Datasheet](https://github.com/Xinyuan-LilyGO/LilyGO-T-SIM7000G)
  - **IN DEVELOPMENT PHASE**: Walter: A certified ESP32-S3 module with LTE-M, NB-IoT, and GNSS for prototyping and production
    - [Product](https://www.crowdsupply.com/dptechnics/walter#products)
  
### LAN - PAN networks
- such as Bluetooth and Wi-Fi provide high bandwidth but have limited coverage and scalability issues.

### LPWANs
#### LoRaWAN
-  **LoRa** is a physical proprietary radio communication technique.
-  **LoRaWAN** (wide area network) defines the communication protocol and system architecture.
- LoRa uses license-free sub-gigahertz radio frequency bands EU868 in EU
- **The technology covers the physical layer**, while other technologies and protocols such as **LoRaWAN (long range wide area network) cover the upper layers: Data Link(MAC), Network(IPv4, IPv6), Transport(TCP, UDP), Session(RPC), Presentation(TLS,SSL), Application(HTTPS, DNS, DHCP, SSH)** 
- LoRa devices have **geolocation capabilities** used for trilaterating positions of devices via timestamps from gateways.
- Data transmitted by an end-node device is received by **multiple gateways: Ethernet, Cellular, WiFi**, which forward the data packets to a centralized network server - LoRaWAN cloud. Data is then forwarded to **application servers.**
- **The Network Server is in charge of the management of LORAWAN Gateways (antennas – “Radio Access Network”)**, the authorization of the sensors and the exchange of data (uplink, downlink) between the sensors and the applications.
- SigFox, the number one alternative to LORAWAN.
- Unlike other LPWANs like Sigfox or NB-IoT, LoRaWAN is more free.
- If you are not within **range of any gateway**, you can simply set up your own. But then the question arises - where to go with her? You can use an existing network (for example TTN community network or perhaps commercial Loriot), connect the gateway to it via the Internet and don't worry about it anymore. Or if you already have your own gateway, why not set up your own private network?
- **private network**: Whether it's problems with internet connectivity (it doesn't even have to be unavailability, but for example company policies). **Sensitive data that must not leave the infrastructure.** Mistrust of the cloud solution.

### Mesh network
#### Zigbee
- **Open Standard**
- is wireless communication technology used to create **personal area networks - PAN**
- The technology defined by the Zigbee specification is intended to be simpler and less expensive than other **wireless personal area networks** (WPANs), such as **Bluetooth or more general wireless networking such as Wi-Fi (or Li-Fi)**.
- Its low power consumption limits transmission distances to **10–100 meters**
- The Zigbee network layer natively supports both **star and tree networks**, and generic mesh networking. **Every network must have one coordinator device.** Within star networks, **the coordinator must be the central node.** Both **trees and meshes allow the use of Zigbee routers to extend communication at the network level.**


#### ZWawe
- **Proprietary Standard**. This can affect factors like **device interoperability**, **ecosystem fragmentation**, **and licensing costs**. 
- is a wireless communications protocol used primarily for **residential and commercial building automation.**
- It is a **mesh network using low-energy radio waves to communicate from device to device**
- **Physical range	100-800 meters**
- **WPANs**


#### RFID
- is the next generation of identifiers designed (not only) to identify goods, following on from the barcode system.
- **Like barcodes, they are used for short-distance contactless communication.** The initiator of the development, as with barcodes, is **Wal-Mart.**
- **RFID technology is used and improved by the newer NFC system, expanding their possibilities and use**


# Notes
- **machine-to-machine** -  is direct communication between devices using any communications channel. Such communication was originally accomplished **by having a remote network of machines relay information back to a central hub - (Star, Network, Tree Topology - Coordinator, Full functional device - FFD, Reduced functional device - RFD) for analysis**, which would then be rerouted into a system like a personal computer, network.
   
- **transceiver** -  is an electronic device which is a combination of a radio **transmitter and a receiver**, hence the name. It can both transmit and receive radio waves using an antenna, for communication purposes. These two related functions are often combined in a single device to reduce manufacturing costs. 

- **Gateway** - active device (network node) that has the **highest position in the computer network.** **The gateway connects two networks working with different communication protocols.** **It also performs the function of a router**, which is why we place it above the router in the sequence of network devices. The designation **default gateway indicates the router** through which the stations reach the external network ussualy to the internet.

