# **1. Project Requirements & Specifications**

**Project Name:** Technical College Campus Network
**Network Topology:** Hierarchical Extended Star (Hub-and-Spoke WAN)

## **A. Building-Specific Requirements**

The network is designed to support the specific operational needs of four major departments. The breakdown of hosts and required hardware is as follows:

### **1. Computer Science (CS) Building**

* **User Groups & Device Count:**
* **Student Labs:** 4 Labs × 25 PCs = **100 Hosts**
* **Faculty (Doctors):** 25 Offices = **25 Hosts**
* **Teaching Assistants (TAs):** 10 Offices = **10 Hosts**
* **Management:** 1 Switch Management IP


* **Total Hosts Required:** **135 End Devices**
* **Infrastructure:**
* 1 Distribution Switch (Layer 3 capable)
* 3 Access Switches (24-port)



### **2. Engineering (ENG) Building**

* **User Groups & Device Count:**
* **Student Labs:** 3 Labs × 30 PCs = **90 Hosts** (High Density)
* **Faculty Offices:** 20 Offices = **20 Hosts**
* **Administration:** 5 Staff PCs = **5 Hosts**
* **Management:** 1 Switch Management IP


* **Total Hosts Required:** **115 End Devices**
* **Infrastructure:**
* 1 Distribution Switch
* 3 Access Switches



### **3. Administration (ADMIN) Building**

* **User Groups & Device Count:**
* **General Staff:** 40 Offices = **40 Hosts**
* **Student Affairs:** 20 PCs = **20 Hosts**
* **Accounts/Financial:** 10 PCs = **10 Hosts**
* **Services (CCTV/Printers):** 10 Units = **10 Hosts**


* **Total Hosts Required:** **80 End Devices**
* **Infrastructure:**
* 1 Distribution Switch
* 2 Access Switches



### **4. Library (LIB) Building**

* **User Groups & Device Count:**
* **Student Research Area:** 60 PCs = **60 Hosts**
* **Library Staff:** 10 PCs = **10 Hosts**
* **Data Center/Servers:** 5 Servers = **5 Hosts**
* **Printers/Scanners:** 5 Units = **5 Hosts**


* **Total Hosts Required:** **80 End Devices**
* **Infrastructure:**
* 1 Distribution Switch
* 2 Access Switches



---

## **B. IP Addressing Plan (VLSM Design)**

The IP addressing scheme utilizes **Variable Length Subnet Masking (VLSM)** to efficiently allocate addresses based on the exact number of hosts per VLAN, ensuring scalability and minimal wastage.

### **1. Campus LAN Addressing (Private Range 10.0.0.0/8)**

| Building | VLAN ID | Subnet Name | Hosts Req. | Network Address | CIDR | Usable IP Range | Broadcast IP |
| --- | --- | --- | --- | --- | --- | --- | --- |
| **CS** | 10 | CS-LABS | 100 | `10.0.0.0` | **/25** | `10.0.0.1` - `10.0.0.126` | `10.0.0.127` |
|  | 11 | CS-FACULTY | 25 | `10.0.0.128` | **/26** | `10.0.0.129` - `10.0.0.190` | `10.0.0.191` |
|  | 12 | CS-TAS | 10 | `10.0.0.192` | **/26** | `10.0.0.193` - `10.0.0.254` | `10.0.0.255` |
| **ENG** | 20 | ENG-LABS | 90 | `10.0.1.0` | **/25** | `10.0.1.1` - `10.0.1.126` | `10.0.1.127` |
|  | 21 | ENG-FACULTY | 20 | `10.0.1.128` | **/27** | `10.0.1.129` - `10.0.1.158` | `10.0.1.159` |
|  | 22 | ENG-ADMIN | 5 | `10.0.1.160` | **/27** | `10.0.1.161` - `10.0.1.190` | `10.0.1.191` |
| **ADMIN** | 30 | ADM-STAFF | 40 | `10.0.2.0` | **/26** | `10.0.2.1` - `10.0.2.62` | `10.0.2.63` |
|  | 31 | ADM-STUDENT | 20 | `10.0.2.64` | **/27** | `10.0.2.65` - `10.0.2.94` | `10.0.2.95` |
|  | 32 | ADM-ACC | 10 | `10.0.2.96` | **/28** | `10.0.2.97` - `10.0.2.110` | `10.0.2.111` |
|  | 33 | ADM-SERV | 10 | `10.0.2.112` | **/28** | `10.0.2.113` - `10.0.2.126` | `10.0.2.127` |
| **LIB** | 40 | LIB-STUDENT | 60 | `10.0.3.0` | **/26** | `10.0.3.1` - `10.0.3.62` | `10.0.3.63` |
|  | 41 | LIB-STAFF | 10 | `10.0.3.64` | **/28** | `10.0.3.65` - `10.0.3.78` | `10.0.3.79` |
|  | 42 | LIB-SERVER | 5 | `10.0.3.80` | **/28** | `10.0.3.81` - `10.0.3.94` | `10.0.3.95` |
|  | 43 | LIB-PRINT | 5 | `10.0.3.96` | **/28** | `10.0.3.97` - `10.0.3.110` | `10.0.3.111` |
| **MGMT** | 99 | MANAGEMENT | N/A | `10.0.254.0` | **/24** | *Subnetted per building* | `10.0.254.255` |

### **2. WAN Backbone (Point-to-Point Connections)**

All WAN links use a **/30** prefix to maximize security and conservation of IP addresses.

| Link Description | Network Address | Subnet Mask | Core Router IP | Remote Router IP |
| --- | --- | --- | --- | --- |
| **Main ↔ CS** | `10.0.10.0` | `255.255.255.252` | `10.0.10.1` | `10.0.10.2` |
| **Main ↔ Engineering** | `10.0.10.4` | `255.255.255.252` | `10.0.10.5` | `10.0.10.6` |
| **Main ↔ Admin** | `10.0.10.8` | `255.255.255.252` | `10.0.10.9` | `10.0.10.10` |
| **Main ↔ Library** | `10.0.10.12` | `255.255.255.252` | `10.0.10.13` | `10.0.10.14` |
| **Main ↔ ISP (Internet)** | `200.1.1.0` | `255.255.255.252` | `200.1.1.1` | `200.1.1.2` |

---

## **C. Final Bill of Materials (BoM)**

Based on the completed design and topology, the following equipment was utilized:

| Device Category | Model (Simulated) | Quantity | Details |
| --- | --- | --- | --- |
| **Routers** | Cisco 2911 / ISR 4331 | **6** | 1 Core, 4 Building, 1 ISP Router. |
| **Distribution Switches** | Cisco Catalyst 3650 | **4** | Layer 3 switches for building aggregation. |
| **Access Switches** | Cisco Catalyst 2960 | **10** | Layer 2 switches for end-user connectivity. |
| **End Devices** | PC / Laptop / Server | **410** | Total user capacity across all VLANs. |
| **Cabling (WAN)** | Serial DTE/DCE | **5** | Connecting Routers via Serial Interfaces. |
| **Cabling (LAN)** | Copper Straight-Through | **~425** | Connecting PCs to Switches & Switches to Routers. |
| **Cabling (Trunks)** | Copper Cross-Over | **14** | Connecting Access Switches to Distribution Switches. |
