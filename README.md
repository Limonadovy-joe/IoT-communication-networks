# IoT Communication Networks

- [Types of IoT Networks](#types-of-iot-networks)
  - [Cellular networks](#cellular-networks)
    - [Advantages of cellular IoT](#advantages-of-cellular-iot)
    - [Types of networks cellular](#types-of-networks-cellular)
    - [Narrowband IoT](#narrowband-iot)
    - [Long term evolution](#long-term-evolution) 


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
- APN stands for **Access Point Name.** It's a configuration setting used by cellular networks to connect a mobile device to a **specific gateway between the carrier's network and the internet or another external network**
- Narrowband-IoT takes advantage of **gaps in the radio frequency spectrum** to provide more efficient connectivity and **prevent interference**. These unused frequency bands are known as **“guard bands.”**
- While **cellular networks like 4G LTE use broadband connections** (which support a wide range of radio frequencies), narrowband connections isolate devices to “narrower” ranges.
- Narrowband-IoT introduces two major power-saving features: **power saving mode (PSM) and discontinuous reception (DRX)**. PSM essentially puts the device to sleep when not in use, and **DRX can extend the period that the device isn’t “actively listening” for a signal.**

#### Long term evolution
- Long term evolution **(LTE-M)**
-  Is an offshoot of LTE technology specifically designed for the Internet of Things.
-  It lets IoT devices connect to 4G networks, **giving them more bandwidth and mobility than NB-IoT**, as well as access to voice over long term evolution **(VoLTE)** — a more advanced voice service.
- Despite the greater power usage, LTE-M can still leverage PSM and DRX to significantly extend a device’s battery life
- When a device needs to transmit or receive a larger volume of data, **LTE-M uses less power than NB-IoT because the higher bandwidth allows it to upload and download data significantly faster.**
- 

  

       

# Notes
- **machine-to-machine** -
- **transceiver** -  is an electronic device which is a combination of a radio **transmitter and a receiver**, hence the name. It can both transmit and receive radio waves using an antenna, for communication purposes. These two related functions are often combined in a single device to reduce manufacturing costs. 
