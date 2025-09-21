# 5G-
The generational evolution

## Standardization

Standardization in telecommunications aims to prevent this kind of problem. When every region develops its own communication technology, it leads to several issues:

Lack of Interoperability: Your phone wouldn't work if you traveled to a different country.

Increased Costs: It's expensive to design and maintain many different systems.

Slower Innovation: Without collaboration, the best ideas from around the world aren't pooled together to create the most efficient technology.

## The Key Players In 5G Standrdization

1. International Telecommunication Union (ITU)

    responsible for all matters related to information and communication technologies

<img width="913" height="485" alt="image" src="https://github.com/user-attachments/assets/c9bf8634-34c3-48b5-9cdd-3975b2e1a861" />


   ###The 5G Requirements
   Peak Data Rate: This is the maximum theoretical speed a single device can achieve in perfect conditions. The target for **5G is 20 Gigabits per second (Gbit/s).**

User Experienced Data Rate: This is the average speed a user can realistically expect in a live network. The goal is to provide **100 Megabits per second (Mbit/s).**

Latency: This measures the delay, or lag, in the network. 5G aims for an extremely low latency of just **1 millisecond (ms)**, which is crucial for applications like real-time communication and autonomous vehicles.

Connection Density: This refers to the number of connected devices the network can support in a given area. 5G is designed to handle a massive **1 million connected devices per square kilometer.**

Mobility: The network must maintain a stable connection for users moving at high speeds. The requirement for 5G is to support seamless connectivity at speeds of up to **500 kilometers per hour (km/h).**

Network Energy Efficiency: This focuses on making the network more environmentally friendly by reducing power consumption. The goal for 5G is a **100-fold improvement in energy efficiency over 4G networks.**

Area Traffic Capacity: This measures the total data traffic the network can handle in a specific area. The target is **10 Megabits per second per square meter (Mbit/s/m²).**

Spectrum Efficiency: This is a measure of how effectively radio frequency is used. 5G is designed to be significantly more efficient than 4G in how it uses the available spectrum.

<img width="1034" height="842" alt="image" src="https://github.com/user-attachments/assets/e9cd0388-d4fe-447f-9bc8-3073c3281a26" />


## The 3rd Generation Partnership Project (3GPP)
the 3GPP figures out the how (the technology to meet those requirements). 3GPP is a global partnership of telecommunications standards organizations from different regions

<img width="1045" height="741" alt="image" src="https://github.com/user-attachments/assets/a9fc0097-e54c-4b81-bf12-8e15873b925d" />

##The Inter-relation between ITU and #3GPP

<img width="1212" height="726" alt="image" src="https://github.com/user-attachments/assets/01b63a8c-55a9-413e-b5de-dc3fc6193e1c" />

3GPP releasess his work every 18 month 

## The 5G user cases

<img width="883" height="584" alt="image" src="https://github.com/user-attachments/assets/f3279d31-520a-4a11-8169-81e0f6926c5e" />

<img width="880" height="529" alt="image" src="https://github.com/user-attachments/assets/eef57a75-efde-40ae-abe8-1a917ad2c7b2" />

<img width="829" height="541" alt="image" src="https://github.com/user-attachments/assets/fb3d3ed5-c3ce-4d0a-a26d-0121b6bfcaf4" />

##Control and User plane Resources

<img width="978" height="588" alt="image" src="https://github.com/user-attachments/assets/7eda2779-7e45-4d2e-b855-3f1cbd8f912d" />

5G RAN:wireless connectivity
UPF:Mobility anchor,Policy enforcement,lawful interception
SMF:session management
AMF:mobility management,registration
AUSF:security
UDM:user subscription data
PCF:session management policies,non session management policies,charging

##5G Development Option

<img width="861" height="514" alt="image" src="https://github.com/user-attachments/assets/0efa6246-a2bf-4537-8517-07ec8de523c5" />

<img width="904" height="558" alt="image" src="https://github.com/user-attachments/assets/0e3dff60-80d6-40a6-b234-df535592e837" />

<img width="1014" height="546" alt="image" src="https://github.com/user-attachments/assets/d529d0fe-285c-456e-9658-0685ebf93aec" />

<img width="891" height="1066" alt="image" src="https://github.com/user-attachments/assets/5dde4acb-742c-44a0-a61f-ebc6bed3fa44" />

<img width="547" height="577" alt="image" src="https://github.com/user-attachments/assets/e3185b5e-7659-4a7a-925b-62c0fb622937" />

<img width="552" height="539" alt="image" src="https://github.com/user-attachments/assets/e4eb97bf-551f-4b92-a14a-7163d98865d2" />

<img width="752" height="550" alt="image" src="https://github.com/user-attachments/assets/c91d3a95-c65c-4e31-b8d1-1cfaf3bd7280" />

Non Standalone(NSA):Non-Standalone (NSA) architecture involves the coexistence of both 4G and 5G network components. This approach allows operators to leverage their existing 4G infrastructure to roll out 5G services more quickly. 

Standalone(SA):A Standalone (SA) architecture uses a single generation of technology for both the radio access and the core network

## The RAN Protocol Stack
<img width="979" height="585" alt="image" src="https://github.com/user-attachments/assets/e1dd2e5f-379d-44b8-842e-b5fa0610de69" />

PHY (Physical Layer): This layer is responsible for the actual transmission of data over the wireless channel. It handles processes like channel coding, modulation, and utilizing multiple antennas to ensure efficient communication.

MAC (Medium Access Control Layer): The MAC layer manages retransmission of data in case of errors. It's also in charge of multiplexing/demultiplexing data from different sources and scheduling data transmissions.

RLC (Radio Link Control Layer): This layer performs segmentation of larger data packets into smaller ones for transmission and reassembles them at the receiving end. It also includes an Automatic Repeat Request (ARQ) mechanism for error correction.

PDCP (Packet Data Convergence Protocol): The PDCP layer is responsible for header compression to reduce the amount of data sent over the air. It also handles ciphering for security and removes duplicate data packets.

SDAP (Service Data Adaptation Protocol): This top layer of the user plane stack is responsible for managing Quality of Service (QoS). It maps different types of data to the appropriate radio bearers to ensure that services like voice calls or video streaming receive the necessary priority.

## Control Plane Protocol Stack

The control plane protocol stack manages the connection and communication between the user's device and the network. It includes many of the same lower layers as the user plane (PDCP, RLC, MAC, PHY), but has two unique upper layers:

RRC (Radio Resource Control): The RRC layer manages the radio resources of the device. This includes broadcasting system information, establishing and managing radio bearers, and configuring measurements for the device to report back to the network.

NAS (Non-access Stratum): The NAS layer handles communication between the user's device and the core network. Its responsibilities include authentication, security, and procedures for when the device is in idle mode.

<img width="963" height="515" alt="image" src="https://github.com/user-attachments/assets/44d90abb-c178-434e-bf05-1aeddb0aa046" />

### For Example
<img width="940" height="537" alt="image" src="https://github.com/user-attachments/assets/04a061ef-758c-456e-b508-b7c42f59dae1" />

## Service Data Adaptation Protocol(SDAP)

<img width="924" height="537" alt="image" src="https://github.com/user-attachments/assets/f21a45d6-e11a-4995-9491-4905f9e06bb5" />

**GBR(Guarantee Bit Rate):** GBR provides a dedicated network resource to ensure a constant data rate for an application.  This is essential for services that need a stable and reliable connection, such as:

Voice and video calls 
Live streaming 
Real-time gaming

**NGBR(Non Guarantee Bit Rate)**:Non-GBR is used for applications that don't require a constant data rate and can tolerate some delays or fluctuations in speed such as:

Web Browsing
Email
File Sharing And Downloads

<img width="957" height="540" alt="image" src="https://github.com/user-attachments/assets/aa976dcf-a971-451a-95dd-711fc55cfaa1" />

### Multiplexing\Demultiplexing

**Multiplexing** is the process of combining multiple signals into a single signal to transmit over a shared medium. **Demultipiplexing** is the reverse process, separating the combined signal back into its original individual signals. In 5G networks, this is managed by the Service Data Adaptation Protocol (SDAP) to handle diverse types of data traffic efficiently.

### Two Types Of Mapping 
**Reflective Mapping**, the device (UE) uses the same mapping for the uplink (UL) that it received in the downlink (DL).

**Explicit Mapping**, This means the device is specifically told which radio bearer to use for a particular QoS flow in the uplink, regardless of the downlink mapping

## Packet Data Convergence Protocol(PDCP):


