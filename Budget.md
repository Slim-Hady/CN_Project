# **Technical College Campus Network - Budget & Equipment Research**


## **1. Network Equipment Specifications & Research**

### **1.1 Routers**

#### **Main Campus Router - Cisco ISR 4331**

| Specification | Details |
|--------------|---------|
| **Model** | Cisco ISR4331/K9 |
| **Description** | Integrated Services Router with 3 GE ports, 2 NIM slots, 1 ISC slot |
| **Throughput** | Up to 100 Mbps (upgradable to 300 Mbps with license) |
| **Features** | Advanced security, SD-WAN capable, modular design |
| **Why Selected** | Ideal as campus core router; supports BGP, OSPF, NAT, and high-density routing |
| **Price** | $3,070.00 USD |
| **Source** | [SecureITStore](https://www.secureitstore.com/isr-4331.asp) |

#### **Building Routers - Cisco 2911**

| Specification | Details |
|--------------|---------|
| **Model** | CISCO2911/K9 |
| **Description** | Integrated Services Router with 3 GE ports, 4 EHWIC slots, 2 DSP slots |
| **Throughput** | Up to 75 Mbps |
| **Features** | Router-on-a-Stick capability, DHCP server, OSPF, Inter-VLAN routing |
| **Why Selected** | Cost-effective for building-level routing; matches project simulation requirements |
| **Price** | $1,567.00 USD |
| **Source** | [Router-Switch.com](https://www.router-switch.com/cisco2911-k9-p-156.html) |

#### **ISP Router - Cisco 2911**

| Specification | Details |
|--------------|---------|
| **Model** | CISCO2911/K9 |
| **Description** | Same as building routers; simulates ISP edge device |
| **Why Selected** | BGP peering capability for external connectivity simulation |
| **Price** | $1,567.00 USD |
| **Source** | [Router-Switch.com](https://www.router-switch.com/cisco2911-k9-p-156.html) |

---

### **1.2 Switches**

#### **Distribution Switches - Cisco Catalyst 3650-24PS-S**

| Specification | Details |
|--------------|---------|
| **Model** | WS-C3650-24PS-S |
| **Description** | 24-Port Gigabit PoE+ Layer 3 Switch with 4x 1G SFP Uplinks |
| **PoE Budget** | 390W |
| **Stacking** | Yes (StackWise-160) |
| **Layer 3 Features** | IP Base:  Static routing, RIP, EIGRP stub, OSPF |
| **Why Selected** | Layer 3 capable for distribution layer; PoE+ for future WAP deployment; high reliability |
| **Price** | $3,289.00 USD |
| **Source** | [ORMSystems](https://www.ormsystems.com/ws-c3650-24ps-s-price.html) |

#### **Access Switches - Cisco Catalyst 2960X-24TS-L**

| Specification | Details |
|--------------|---------|
| **Model** | WS-C2960X-24TS-L |
| **Description** | 24-Port Gigabit Ethernet Switch with 4x 1G SFP Uplinks |
| **Management** | LAN Base (basic L2 features, VLAN, STP, Port Security) |
| **Features** | FlexStack-Plus stacking, Energy Efficient Ethernet |
| **Why Selected** | Industry-standard access layer switch; Port Security, VLAN support, SSH management |
| **Price** | $1,584.00 USD |
| **Source** | [Newegg](https://www.newegg.com/cisco-2960x-24ts-l/p/N82E16833420518) |

---

### **1.3 Cabling Infrastructure**

#### **WAN Serial Cables - Cisco Smart Serial DTE/DCE**

| Specification | Details |
|--------------|---------|
| **Model** | CAB-SS-2626X-3 (3ft) |
| **Description** | Smart Serial Crossover Cable for WIC-2T interfaces |
| **Why Selected** | Required for serial WAN connections between routers |
| **Price** | $9. 40 USD |
| **Source** | [Amazon](https://www.amazon.com/EDIMS-Length-Router-CAB-SS-2626X-Serial/dp/B06VXVCM32) |

#### **LAN Cabling - Cat6 Bulk Ethernet Cable (1000ft)**

| Specification | Details |
|--------------|---------|
| **Type** | Cat6 UTP Riser-Rated (CMR) Solid Copper |
| **Speed Support** | 1 Gbps (up to 10 Gbps for short runs) |
| **Why Selected** | Future-proof Gigabit infrastructure; industry standard for campus networks |
| **Price** | $139.99 USD per 1000ft box |
| **Source** | [TS Cables](https://tscables.com/collections/cat6-bulk-cable) |

#### **Cat6 Patch Cables (Pre-made 5ft)**

| Specification | Details |
|--------------|---------|
| **Type** | Cat6 UTP Snagless Patch Cable |
| **Length** | 5ft (1.5m) |
| **Why Selected** | Pre-terminated for quick deployment; connects end devices to wall jacks |
| **Price** | $3.99 USD each |
| **Source** | [Monoprice](https://www.monoprice.com/) |

#### **Fiber Patch Cables (LC-LC Single Mode)**

| Specification | Details |
|--------------|---------|
| **Type** | OS2 Single Mode Duplex LC-LC |
| **Length** | 3 meters |
| **Why Selected** | Required for SFP uplinks between distribution switches |
| **Price** | $8.00 USD each |
| **Source** | [FS.com](https://www.fs.com/) |

---

### **1.4 SFP Transceiver Modules**

| Specification | Details |
|--------------|---------|
| **Model** | 1000BASE-LX SFP (Cisco Compatible) |
| **Description** | 1 Gigabit SFP module for single-mode fiber uplinks |
| **Why Selected** | Required for switch-to-switch fiber uplinks between distribution and access layers |
| **Price** | $18.00 USD each |
| **Source** | [FS.com](https://www.fs.com/products/29849. html) |

---

### **1.5 Infrastructure & Accessories**

#### **Network Racks - 42U Server Cabinet**

| Specification | Details |
|--------------|---------|
| **Size** | 42U (Standard 19" width) |
| **Features** | Lockable doors, cable management, cooling fans, casters |
| **Why Selected** | Houses routers, switches, and patch panels in each building's network closet |
| **Price** | $1,249.00 USD |
| **Source** | [Amazon - Tecmojo](https://www.amazon.com/Tecmojo-Network-Enclosure-Networking-Equipment/dp/B0DF29G9VQ) |

#### **Patch Panels - 24-Port Cat6**

| Specification | Details |
|--------------|---------|
| **Type** | Cat6 RJ45 110-Style Punch-Down |
| **Size** | 1U Rack Mountable |
| **Why Selected** | Organizes cable terminations in each network closet |
| **Price** | $55.00 USD each |
| **Source** | [Cable Matters](https://www.cablematters.com/pc-334-159-ul-listed-rackmount-or-wallmount-24-port-cat6-rj45-patch-panel.aspx) |

#### **Cable Management - Horizontal Organizer**

| Specification | Details |
|--------------|---------|
| **Type** | 1U Horizontal Cable Manager |
| **Why Selected** | Maintains organized cabling in racks |
| **Price** | $20.00 USD each |
| **Source** | [Amazon](https://www.amazon.com/) |

---

### **1.6 Power Equipment**

#### **UPS Backup - APC Smart-UPS 1500VA**

| Specification | Details |
|--------------|---------|
| **Model** | SMT1500C |
| **Capacity** | 1500VA / 1000W |
| **Runtime** | ~24 minutes at half load |
| **Features** | Pure sinewave, LCD, SmartConnect cloud monitoring, AVR |
| **Why Selected** | Protects network equipment from power outages; critical for router/switch uptime |
| **Price** | $619.99 USD |
| **Source** | [Amazon](https://www.amazon.com/APC-Smart-UPS-SmartConnect-Uninterruptible-SMT1500C/dp/B0762QJ6Y1) |

#### **PDU - Rack Mount Power Distribution Unit**

| Specification | Details |
|--------------|---------|
| **Type** | Basic Rack PDU, 1U, 8 Outlets |
| **Why Selected** | Distributes power to rack-mounted equipment |
| **Price** | $75.00 USD each |
| **Source** | [Amazon](https://www.amazon.com/) |

---

### **1.7 Accessories**

#### **Console Cables**

| Specification | Details |
|--------------|---------|
| **Type** | USB to RJ45 Console Cable |
| **Why Selected** | Required for initial router/switch configuration |
| **Price** | $12.00 USD each |
| **Source** | [Amazon](https://www.amazon.com/) |

#### **Network Tool Kit**

| Specification | Details |
|--------------|---------|
| **Contents** | RJ45 Crimping tool, Punch-down tool, Cable tester, Wire stripper |
| **Why Selected** | Essential for cable termination and testing |
| **Price** | $120.00 USD |
| **Source** | [Amazon](https://www.amazon.com/) |

#### **Cable Labels**

| Specification | Details |
|--------------|---------|
| **Type** | Self-adhesive cable labels and markers |
| **Why Selected** | Professional cable identification and documentation |
| **Price** | $35.00 USD |
| **Source** | [Amazon](https://www.amazon.com/) |

---

## **2. Detailed Budget Table**

| Category | Item | Model/Specification | Qty | Unit Price (USD) | Total Cost (USD) |
|----------|------|---------------------|-----|------------------|------------------|
| **ROUTERS** | | | | | |
| | Main Campus Router | Cisco ISR 4331 (ISR4331/K9) | 1 | $3,070.00 | $3,070.00 |
| | Building Routers | Cisco 2911 (CISCO2911/K9) | 4 | $1,567.00 | $6,268.00 |
| | ISP Router | Cisco 2911 (CISCO2911/K9) | 1 | $1,567.00 | $1,567.00 |
| | | | | **Routers Subtotal** | **$10,905.00** |
| **SWITCHES** | | | | | |
| | Distribution Switches | Cisco Catalyst 3650-24PS-S | 4 | $3,289.00 | $13,156.00 |
| | Access Switches | Cisco Catalyst 2960X-24TS-L | 10 | $1,584.00 | $15,840.00 |
| | | | | **Switches Subtotal** | **$28,996.00** |
| **CABLING** | | | | | |
| | WAN Serial Cables | Cisco CAB-SS-2626X (DTE/DCE) 3ft | 5 | $9.40 | $47. 00 |
| | Cat6 Bulk Cable | Cat6 UTP CMR 1000ft boxes | 5 | $139.99 | $699.95 |
| | Cat6 Patch Cables | Pre-terminated 5ft | 450 | $3.99 | $1,795.50 |
| | Fiber Patch Cables | LC-LC Single Mode 3m | 14 | $8.00 | $112.00 |
| | | | | **Cabling Subtotal** | **$2,654.45** |
| **TRANSCEIVERS** | | | | | |
| | SFP Modules | 1000BASE-LX SFP (Compatible) | 28 | $18.00 | $504.00 |
| | | | | **Transceivers Subtotal** | **$504.00** |
| **INFRASTRUCTURE** | | | | | |
| | Network Racks | 42U Server Cabinet (Tecmojo) | 4 | $1,249.00 | $4,996.00 |
| | Patch Panels | 24-Port Cat6 RJ45 | 14 | $55.00 | $770.00 |
| | Cable Management | 1U Horizontal Cable Organizers | 14 | $20.00 | $280.00 |
| | | | | **Infrastructure Subtotal** | **$6,046.00** |
| **POWER** | | | | | |
| | UPS Systems | APC Smart-UPS 1500VA (SMT1500C) | 5 | $619.99 | $3,099.95 |
| | PDU | Rack-mount PDU 8-outlet | 5 | $75.00 | $375.00 |
| | | | | **Power Subtotal** | **$3,474.95** |
| **ACCESSORIES** | | | | | |
| | Console Cables | USB to RJ45 Console | 6 | $12.00 | $72.00 |
| | Network Tool Kit | Crimping, punch-down, tester | 1 | $120.00 | $120.00 |
| | Cable Labels | Self-adhesive labels and markers | 1 | $35.00 | $35.00 |
| | | | | **Accessories Subtotal** | **$227.00** |
| | | | | | |
| | | | | **EQUIPMENT TOTAL** | **$52,807.40** |
| | | | | | |
| **ADDITIONAL COSTS** | | | | | |
| | Shipping & Handling | Estimated 5% of equipment | | | $2,640.37 |
| | Contingency | Unexpected costs (10%) | | | $5,280.74 |
| | | | | **Additional Subtotal** | **$7,921.11** |
| | | | | | |
| | | | | **GRAND TOTAL** | **$60,728.51** |

---

## **3. Cost Summary by Category**

| Category | Total Cost (USD) | Percentage |
|----------|------------------|------------|
| Routers | $10,905.00 | 18.0% |
| Switches | $28,996.00 | 47.7% |
| Cabling | $2,654.45 | 4.4% |
| Transceivers | $504.00 | 0.8% |
| Infrastructure | $6,046.00 | 10.0% |
| Power | $3,474.95 | 5.7% |
| Accessories | $227.00 | 0.4% |
| Shipping & Contingency | $7,921.11 | 13.0% |
| **TOTAL** | **$60,728.51** | **100%** |

---

## **4. Equipment Justification**

### **Why These Specific Models Were Selected:**

| Equipment | Justification |
|-----------|---------------|
| **Cisco ISR 4331** | Modern campus core router with high throughput; supports all required protocols (BGP, OSPF, NAT); modular for future expansion |
| **Cisco 2911** | Matches Packet Tracer simulation; supports Router-on-a-Stick, DHCP, ACLs, SSH; cost-effective for building-level deployment |
| **Cisco Catalyst 3650** | Layer 3 distribution switch with PoE+ for future wireless; stacking capability for redundancy; enterprise-grade reliability |
| **Cisco Catalyst 2960X** | Industry-standard access switch; full VLAN, Port Security, and SSH support; proven reliability in education environments |
| **Cat6 Cabling** | Supports current Gigabit and future 10 Gigabit requirements; industry standard for new installations |
| **APC Smart-UPS 1500VA** | Enterprise-grade power protection; sufficient capacity for router + switch per building; remote monitoring capability |
| **42U Racks** | Standard size accommodates all equipment with room for growth; professional cable management and security |

---

## **5. Warranty Information**

| Equipment | Warranty Period | Support Level |
|-----------|-----------------|---------------|
| Cisco ISR 4331 | 90 Days (Limited Lifetime with SmartNet) | Hardware replacement |
| Cisco 2911 | 90 Days | Hardware replacement |
| Cisco Catalyst 3650 | 90 Days (Limited Lifetime with SmartNet) | Hardware replacement |
| Cisco Catalyst 2960X | Limited Lifetime | Hardware replacement |
| APC Smart-UPS | 3 Years | Repair or replace |
| Cabling & Accessories | 1 Year | Manufacturer warranty |

---

## **6. Pricing Sources**

| Item | Source | URL |
|------|--------|-----|
| Cisco ISR 4331 | SecureITStore | https://www.secureitstore.com/isr-4331.asp |
| Cisco 2911 | Router-Switch.com | https://www.router-switch.com/cisco2911-k9-p-156.html |
| Cisco Catalyst 3650-24PS-S | ORMSystems | https://www.ormsystems.com/ws-c3650-24ps-s-price.html |
| Cisco Catalyst 2960X-24TS-L | Newegg | https://www.newegg.com/cisco-2960x-24ts-l/p/N82E16833420518 |
| Serial DTE/DCE Cables | Amazon | https://www.amazon.com/ |
| Cat6 Bulk Cable | TS Cables | https://tscables.com/collections/cat6-bulk-cable |
| SFP Transceivers | FS. com | https://www.fs.com/products/29849.html |
| 42U Server Cabinet | Amazon (Tecmojo) | https://www.amazon.com/ |
| Patch Panels | Cable Matters | https://www.cablematters.com/ |
| APC Smart-UPS 1500VA | Amazon | https://www.amazon.com/ |

---


## **8. Alternative Cost-Saving Options**

For budget-constrained implementations, consider:

| Option | Potential Savings |
|--------|-------------------|
| Refurbished Cisco 2911 routers (~$175 each) | Save ~$5,568 |
| Refurbished Catalyst 3650 switches (~$600 each) | Save ~$10,756 |
| Refurbished Catalyst 2960X switches (~$250 each) | Save ~$13,340 |
| **Total Potential Savings with Refurbished Equipment** | **~$29,664** |

**Note:** Refurbished equipment may have limited warranty (90 days typical) and shorter remaining lifespan.

---
