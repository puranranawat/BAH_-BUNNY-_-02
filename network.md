# Task 4.1 – Network Design for Truelec

## 1. Assumptions
This network design is based on the following assumptions:
- Headquarters (HQ) location: <<HQ_CITY>>
- Branch office locations: <<BRANCH_CITY_1>>, <<BRANCH_CITY_2>>, <<BRANCH_CITY_3>>
- Total number of staff at HQ: <<HQ_STAFF_COUNT>> staff
- Total number of staff at one branch office: <<BRANCH_STAFF_COUNT>> staff

## 2. Business Requirements Summary
Truelec needs a fast and secure network to support daily business work in the headquarters and branches. The network must support wired computers, WiFi for staff devices, and guest WiFi for visitors. The company also uses CCTV cameras, RFID systems, and IoT devices, so these devices must be connected safely. The network must support a booking application that runs on servers, and it must allow HQ and branch offices to communicate securely using WAN connections.

## 3. Network Design Overview
We designed the Truelec network using a structured and secure model. The network is divided into multiple VLANs to separate traffic for staff, servers, guests, and IoT devices. This helps reduce security risks and improves network management. A firewall is used to protect the internal network. A secure VPN tunnel is used to connect HQ and branch offices. Redundancy is included in WAN connectivity to reduce downtime.

## 4. HQ Network Design

### 4.1 HQ Network Diagram
(Insert HQ network diagram image here)
File: diagrams/HQ_Network.png

### 4.2 HQ Design Explanation (Justification)
At HQ, we used a layered network approach with a main router, firewall, core switch, and access switches. The firewall protects the network from external threats and controls access between VLANs. Servers are placed in a separate VLAN to keep them secure. Staff computers are placed in a staff VLAN. Guest WiFi is separated so visitors cannot access internal systems. CCTV and IoT devices are also separated to reduce the risk of device hacking.

### 4.3 HQ VLAN / Subnet Plan
The following VLANs are used in the headquarters:
- VLAN 10: Staff Wired Network
- VLAN 20: Staff WiFi Network
- VLAN 30: Guest WiFi Network
- VLAN 40: Server Network
- VLAN 50: CCTV / RFID / IoT Network
- VLAN 99: Network Management

## 5. Branch Office Network Design

### 5.1 Branch Network Diagram
(Insert branch network diagram image here)
File: diagrams/Branch_Network.png

### 5.2 Branch Design Explanation (Justification)
The branch office uses a smaller but similar design as HQ. A branch router connects to the internet and creates a secure VPN connection to HQ. A firewall policy is applied to secure traffic. The branch office has a switch and WiFi access points for staff. Guest WiFi and IoT devices are separated using VLANs. This improves security and reduces the chance of internal attacks.

## 6. WAN Connectivity Design
We used a secure WAN design that connects the branch office to HQ. A site-to-site VPN tunnel is used to encrypt traffic between the locations. This helps protect customer and business data during transmission. A backup internet link is suggested for HQ so business services can continue even if the main ISP fails.

## 7. WiFi Design

### 7.1 WiFi Requirements
Truelec needs WiFi for staff devices like laptops and phones. Truelec also needs guest WiFi for visitors, but guest users must not access internal systems.

### 7.2 WiFi Settings (with values)
We used the following WiFi settings:
- Staff SSID name: Truelec-Staff
- Staff WiFi security: WPA3 (fallback WPA2)
- Staff authentication: Strong password + changed every 90 days
- Guest SSID name: Truelec-Guest
- Guest WiFi security: WPA2
- Guest authentication: Guest password changed weekly
- Guest access rule: Internet only (no access to internal VLANs)
- Channel plan: Automatic channel selection to reduce interference
- AP placement: APs placed in central areas for full coverage

### 7.3 Access Point Placement Justification
Access points are placed in office open areas, meeting rooms, and reception areas to provide strong signal coverage. This reduces dead zones and helps staff remain connected while moving within the office.

## 8. IPv4 Address Allocation Plan

### 8.1 IP Addressing Rules Followed
We followed the IP addressing requirements:
- Subnet masks used: /16 and /24 only
- First octet is based on student ID last 2 digits: <<STUDENT1_ID_LAST2>>
- Private IP ranges such as 192.168.x.x were not used

### 8.2 HQ IP Plan
We used the following IP subnets for HQ:
- HQ Staff Wired (VLAN 10): <<ID>>.10.10.0/24
- HQ Staff WiFi (VLAN 20): <<ID>>.10.20.0/24
- HQ Guest WiFi (VLAN 30): <<ID>>.10.30.0/24
- HQ Servers (VLAN 40): <<ID>>.10.40.0/24
- HQ CCTV/IoT (VLAN 50): <<ID>>.10.50.0/24
- HQ Management (VLAN 99): <<ID>>.10.99.0/24

## 8.3 Branch IP Plan
We used the following IP subnets for the branch office:
- Branch Staff (VLAN 10): <<ID>>.20.10.0/24
- Branch WiFi (VLAN 20): <<ID>>.20.20.0/24
- Branch Guest WiFi (VLAN 30): <<ID>>.20.30.0/24
- Branch Servers (VLAN 40): <<ID>>.20.40.0/24
- Branch CCTV/IoT (VLAN 50): <<ID>>.20.50.0/24
- Branch Management (VLAN 99): <<ID>>.20.99.0/24

## 9. Recommended Hardware List (With AUD Prices)
The following hardware is recommended for the network:

| Device | Purpose | Minimum Specs | Example Model | Price (AUD) | Link |
|--------|---------|--------------|--------------|-------------|------|
| Router | WAN and VPN | VPN support, dual WAN | <<MODEL>> | <<PRICE>> | <<LINK>> |
| Firewall | Security | Stateful firewall, VLAN support | <<MODEL>> | <<PRICE>> | <<LINK>> |
| Core Switch | HQ switching | Managed L2/L3 | <<MODEL>> | <<PRICE>> | <<LINK>> |
| Access Switch | User devices | Managed VLAN support | <<MODEL>> | <<PRICE>> | <<LINK>> |
| WiFi AP | Wireless access | WPA3, dual band | <<MODEL>> | <<PRICE>> | <<LINK>> |
| Server | Booking app | Multi-core CPU, SSD | <<MODEL>> | <<PRICE>> | <<LINK>> |

## 10. Conclusion
In conclusion, this network design provides Truelec with a secure, scalable, and reliable network. The design separates different types of users and devices using VLANs and subnets. It protects business systems using firewall security and encrypted VPN connectivity. This design also supports current needs and future growth for HQ and branch offices.
