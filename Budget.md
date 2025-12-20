# **Technical College Campus Network - Budget & Equipment Research**

---

## **1. Network Equipment Specifications & Research**

### **1.1 Routers**

#### **Core Router - Cisco ISR 4331**

| Specification | Details |
|--------------|---------|
| **Model** | Cisco ISR4331/K9 |
| **Description** | Integrated Services Router with 3 GE ports, 2 NIM slots |
| **Role in Project** | Main Campus Router - Central backbone connecting all buildings |
| **Features Used** | OSPF Area 0, BGP (AS 65000), NAT Overload, Default Route Distribution |
| **Price** | 46,779 EGP |
| **Source** | [ServerBasket Egypt](https://www.serverbasket.net/eg/p/cisco-isr-4331-router/) |

#### **Building & ISP Routers - Cisco 2911**

| Specification | Details |
|--------------|---------|
| **Model** | CISCO2911/K9 |
| **Description** | Integrated Services Router with 3 GE ports, 4 EHWIC slots |
| **Role in Project** | CS Router, ENG Router, ADMIN Router, LIB Router, ISP Router |
| **Features Used** | Router-on-a-Stick (802.1Q), DHCP Server, OSPF, ACLs, BGP (ISP) |
| **Price** | 12,500 EGP each |
| **Source** | [Server Switch Egypt](https://www.serverswitch. net/ar/shop/cisco2911-k9-cisco-2911-router-isr-g2-cisco2911-k9-643) |

---

### **1.2 Switches**

#### **Distribution Switches - Cisco Catalyst 3650**

| Specification | Details |
|--------------|---------|
| **Model** | WS-C3650-24PS-S |
| **Description** | 24-Port Gigabit PoE+ Layer 3 Switch |
| **Role in Project** | Building aggregation layer (1 per building) |
| **Features Used** | VLAN creation, 802.1Q Trunking, Management VLAN 99 |
| **Price** | 13,500 EGP each |
| **Source** | [IGFI Egypt](https://igfi.me/product_brand/cisco/) |

#### **Access Switches - Cisco Catalyst 2960**

| Specification | Details |
|--------------|---------|
| **Model** | WS-C2960-24TT-L |
| **Description** | 24-Port Fast Ethernet Layer 2 Switch |
| **Role in Project** | End-user connectivity in each building |
| **Features Used** | VLAN assignment, Port Security, 802.1Q Trunking, PortFast, SSH |
| **Price** | 10,000 EGP each |
| **Source** | [Dubizzle Egypt](https://www.dubizzle. com. eg/) |

---

### **1.3 Cabling**

| Cable Type | Description | Price (EGP) | Source |
|------------|-------------|-------------|--------|
| **Serial DTE/DCE** | WAN connections between routers | 500 EGP each | [Amazon Egypt](https://www.amazon.eg/) |
| **Cat6 Patch Cable (3m)** | PC-to-Switch connections | 100 EGP each | [Jumia Egypt](https://www.jumia.com.eg/cat-6-cables/) |
| **Cat6 Cross-Over (3m)** | Switch-to-Switch trunk connections | 120 EGP each | [Jumia Egypt](https://www.jumia.com.eg/cat-6-cables/) |

---

### **1.4 End Devices**

| Device Type | Description | Price (EGP) | Source |
|-------------|-------------|-------------|--------|
| **Desktop PC** | Dell Optiplex 7050 (Core i5, 8GB, 256GB SSD) | 9,600 EGP each | [Pricena Egypt](https://eg.pricena. com/) |
| **Server** | Dell PowerEdge R250 Rack Server | 40,387 EGP each | [ServerBasket Egypt](https://www.serverbasket.net/eg/c/dell-servers/) |
| **Network Printer** | HP LaserJet Pro MFP M141W | 7,000 EGP each | [Jumia Egypt](https://www.jumia.com.eg/printers/hp/) |
| **CCTV Camera** | Hikvision 2MP IP Camera | 1,200 EGP each | [Jumia Egypt](https://www.jumia.com.eg/mlp-ip-camera/) |

---

## **2. Per-Building Budget Breakdown**

### **2.1 Computer Science (CS) Building**

**End Devices:**
- Student Labs: 4 Labs × 25 PCs = 100 PCs
- Faculty Offices: 25 PCs
- Teaching Assistants: 10 PCs
- **Total:  135 End Devices**

**Infrastructure:**
- 1 Router (Cisco 2911)
- 1 Distribution Switch (Catalyst 3650)
- 3 Access Switches (Catalyst 2960)

| Item | Model | Qty | Unit Price (EGP) | Total (EGP) |
|------|-------|-----|------------------|-------------|
| Building Router | Cisco 2911 | 1 | 12,500 | 12,500 |
| Distribution Switch | Catalyst 3650 | 1 | 13,500 | 13,500 |
| Access Switches | Catalyst 2960 | 3 | 10,000 | 30,000 |
| Trunk Cables (Cross-Over) | Cat6 | 3 | 120 | 360 |
| Router-to-Switch Cable | Cat6 | 1 | 100 | 100 |
| **Infrastructure Subtotal** | | | | **56,460** |
| Desktop PCs (Labs) | Dell Optiplex | 100 | 9,600 | 960,000 |
| Desktop PCs (Faculty) | Dell Optiplex | 25 | 9,600 | 240,000 |
| Desktop PCs (TAs) | Dell Optiplex | 10 | 9,600 | 96,000 |
| LAN Cables (End Devices) | Cat6 | 135 | 100 | 13,500 |
| **End Devices Subtotal** | | | | **1,309,500** |
| | | | **CS Building Total** | **1,365,960 EGP** |

---

### **2.2 Engineering (ENG) Building**

**End Devices:**
- Student Labs:  3 Labs × 30 PCs = 90 PCs
- Faculty Offices:  20 PCs
- Administration: 5 PCs
- **Total: 115 End Devices**

**Infrastructure:**
- 1 Router (Cisco 2911)
- 1 Distribution Switch (Catalyst 3650)
- 3 Access Switches (Catalyst 2960)

| Item | Model | Qty | Unit Price (EGP) | Total (EGP) |
|------|-------|-----|------------------|-------------|
| Building Router | Cisco 2911 | 1 | 12,500 | 12,500 |
| Distribution Switch | Catalyst 3650 | 1 | 13,500 | 13,500 |
| Access Switches | Catalyst 2960 | 3 | 10,000 | 30,000 |
| Trunk Cables (Cross-Over) | Cat6 | 3 | 120 | 360 |
| Router-to-Switch Cable | Cat6 | 1 | 100 | 100 |
| **Infrastructure Subtotal** | | | | **56,460** |
| Desktop PCs (Labs) | Dell Optiplex | 90 | 9,600 | 864,000 |
| Desktop PCs (Faculty) | Dell Optiplex | 20 | 9,600 | 192,000 |
| Desktop PCs (Admin) | Dell Optiplex | 5 | 9,600 | 48,000 |
| LAN Cables (End Devices) | Cat6 | 115 | 100 | 11,500 |
| **End Devices Subtotal** | | | | **1,115,500** |
| | | | **ENG Building Total** | **1,171,960 EGP** |

---

### **2.3 Administration (ADMIN) Building**

**End Devices:**
- General Staff: 40 PCs
- Student Affairs: 20 PCs
- Accounts/Financial: 10 PCs
- Services (CCTV/Printers): 10 Units
- **Total:  80 End Devices**

**Infrastructure:**
- 1 Router (Cisco 2911)
- 1 Distribution Switch (Catalyst 3650)
- 2 Access Switches (Catalyst 2960)

| Item | Model | Qty | Unit Price (EGP) | Total (EGP) |
|------|-------|-----|------------------|-------------|
| Building Router | Cisco 2911 | 1 | 12,500 | 12,500 |
| Distribution Switch | Catalyst 3650 | 1 | 13,500 | 13,500 |
| Access Switches | Catalyst 2960 | 2 | 10,000 | 20,000 |
| Trunk Cables (Cross-Over) | Cat6 | 2 | 120 | 240 |
| Router-to-Switch Cable | Cat6 | 1 | 100 | 100 |
| **Infrastructure Subtotal** | | | | **46,340** |
| Desktop PCs (Staff) | Dell Optiplex | 40 | 9,600 | 384,000 |
| Desktop PCs (Student Affairs) | Dell Optiplex | 20 | 9,600 | 192,000 |
| Desktop PCs (Accounts) | Dell Optiplex | 10 | 9,600 | 96,000 |
| CCTV Cameras | Hikvision 2MP | 5 | 1,200 | 6,000 |
| Network Printers | HP LaserJet | 5 | 7,000 | 35,000 |
| LAN Cables (End Devices) | Cat6 | 80 | 100 | 8,000 |
| **End Devices Subtotal** | | | | **721,000** |
| | | | **ADMIN Building Total** | **767,340 EGP** |

---

### **2.4 Library (LIB) Building**

**End Devices:**
- Student Research Area: 60 PCs
- Library Staff: 10 PCs
- Data Center/Servers: 5 Servers
- Printers/Scanners: 5 Units
- **Total: 80 End Devices**

**Infrastructure:**
- 1 Router (Cisco 2911)
- 1 Distribution Switch (Catalyst 3650)
- 2 Access Switches (Catalyst 2960)

| Item | Model | Qty | Unit Price (EGP) | Total (EGP) |
|------|-------|-----|------------------|-------------|
| Building Router | Cisco 2911 | 1 | 12,500 | 12,500 |
| Distribution Switch | Catalyst 3650 | 1 | 13,500 | 13,500 |
| Access Switches | Catalyst 2960 | 2 | 10,000 | 20,000 |
| Trunk Cables (Cross-Over) | Cat6 | 2 | 120 | 240 |
| Router-to-Switch Cable | Cat6 | 1 | 100 | 100 |
| **Infrastructure Subtotal** | | | | **46,340** |
| Desktop PCs (Research) | Dell Optiplex | 60 | 9,600 | 576,000 |
| Desktop PCs (Staff) | Dell Optiplex | 10 | 9,600 | 96,000 |
| Servers (Data Center) | Dell PowerEdge R250 | 5 | 40,387 | 201,935 |
| Network Printers/Scanners | HP LaserJet | 5 | 7,000 | 35,000 |
| LAN Cables (End Devices) | Cat6 | 80 | 100 | 8,000 |
| **End Devices Subtotal** | | | | **916,935** |
| | | | **LIB Building Total** | **963,275 EGP** |

---

### **2.5 Core Infrastructure (Main Campus & ISP)**

| Item | Model | Qty | Unit Price (EGP) | Total (EGP) |
|------|-------|-----|------------------|-------------|
| Main Campus Router | Cisco ISR 4331 | 1 | 46,779 | 46,779 |
| ISP Router | Cisco 2911 | 1 | 12,500 | 12,500 |
| WAN Serial Cables | DTE/DCE | 5 | 500 | 2,500 |
| | | | **Core Infrastructure Total** | **61,779 EGP** |

---

## **3. Complete Budget Summary**

### **3.1 By Building**

| Building | Infrastructure (EGP) | End Devices (EGP) | **Total (EGP)** |
|----------|----------------------|-------------------|-----------------|
| **Computer Science (CS)** | 56,460 | 1,309,500 | **1,365,960** |
| **Engineering (ENG)** | 56,460 | 1,115,500 | **1,171,960** |
| **Administration (ADMIN)** | 46,340 | 721,000 | **767,340** |
| **Library (LIB)** | 46,340 | 916,935 | **963,275** |
| **Core (Main + ISP)** | 61,779 | - | **61,779** |
| | | **GRAND TOTAL** | **4,330,314 EGP** |

---

### **3.2 By Category**

| Category | Quantity | Total Cost (EGP) | Percentage |
|----------|----------|------------------|------------|
| **Routers** | 6 | 109,279 | 2.5% |
| **Distribution Switches** | 4 | 54,000 | 1.2% |
| **Access Switches** | 10 | 100,000 | 2.3% |
| **Desktop PCs** | 390 | 3,744,000 | 86.5% |
| **Servers** | 5 | 201,935 | 4.7% |
| **Printers** | 10 | 70,000 | 1.6% |
| **CCTV Cameras** | 5 | 6,000 | 0.1% |
| **Cabling** | ~444 | 45,100 | 1.1% |
| **TOTAL** | | **4,330,314 EGP** | **100%** |

---

### **3.3 Network Infrastructure Only (Excluding End Devices)**

| Category | Quantity | Total Cost (EGP) |
|----------|----------|------------------|
| Routers | 6 | 109,279 |
| Distribution Switches | 4 | 54,000 |
| Access Switches | 10 | 100,000 |
| Cabling | ~444 | 45,100 |
| **INFRASTRUCTURE TOTAL** | | **308,379 EGP** |

---

## **4. Equipment  Table**

| Device Category | Model | Qty | Unit Price (EGP) | Total (EGP) |
|-----------------|-------|-----|------------------|-------------|
| **Routers** | Cisco ISR 4331 | 1 | 46,779 | 46,779 |
| | Cisco 2911 | 5 | 12,500 | 62,500 |
| **Distribution Switches** | Cisco Catalyst 3650 | 4 | 13,500 | 54,000 |
| **Access Switches** | Cisco Catalyst 2960 | 10 | 10,000 | 100,000 |
| **Cabling (WAN)** | Serial DTE/DCE | 5 | 500 | 2,500 |
| **Cabling (LAN)** | Cat6 Straight-Through | ~425 | 100 | 42,500 |
| **Cabling (Trunks)** | Cat6 Cross-Over | 14 | 120 | 1,680 |
| **Desktop PCs** | Dell Optiplex 7050 | 390 | 9,600 | 3,744,000 |
| **Servers** | Dell PowerEdge R250 | 5 | 40,387 | 201,935 |
| **Printers** | HP LaserJet Pro MFP | 10 | 7,000 | 70,000 |
| **CCTV Cameras** | Hikvision 2MP IP | 5 | 1,200 | 6,000 |
| | | | **GRAND TOTAL** | **4,331,894 EGP** |

---

## **5. Pricing Sources**

| Item | Source |
|------|--------|
| Cisco ISR 4331 | [ServerBasket Egypt](https://www.serverbasket.net/eg/p/cisco-isr-4331-router/) |
| Cisco 2911 | [Server Switch Egypt](https://www.serverswitch.net/) |
| Cisco Catalyst 3650 | [IGFI Egypt](https://igfi.me/product_brand/cisco/) |
| Cisco Catalyst 2960 | [Dubizzle Egypt](https://www.dubizzle.com. eg/) |
| Cat6 Ethernet Cables | [Jumia Egypt](https://www.jumia.com.eg/cat-6-cables/) |
| Dell Desktop PCs | [Pricena Egypt](https://eg.pricena.com/) |
| Dell Servers | [ServerBasket Egypt](https://www.serverbasket. net/eg/c/dell-servers/) |
| HP Printers | [Jumia Egypt](https://www.jumia.com.eg/printers/hp/) |
| CCTV Cameras | [Jumia Egypt](https://www.jumia.com. eg/mlp-ip-camera/) |
| Serial Cables | [Amazon Egypt](https://www.amazon.eg/) |

---

