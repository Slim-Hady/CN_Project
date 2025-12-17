# TEST 1: ISP Router Connectivity

``` show ip interface brief ``` 
Expected Result:
```
Interface        IP-Address      OK? Method Status
Lo0              8.8.8.8         YES manual up  
Se0/0/0          200.1.1.2       YES manual up
```
What we're testing: ISP interfaces are up with correct IPs

<img width="791" height="405" alt="image" src="https://github.com/user-attachments/assets/bfc48dc9-3e96-4007-9880-434f1fe83d75" />


# TEST 2: Main Router WAN Connection : 

```ping 200.1.1.2```

Expected:
````
Type escape sequence to abort.
Sending 5, 100-byte ICMP Echos to 200.1.1.2, timeout is 2 seconds:
!!!!!
Success rate is 100 percent (5/5)
````

What we're testing: Physical connectivity to ISP

<img width="791" height="405" alt="image" src="https://github.com/user-attachments/assets/62686ec7-3979-4a76-911d-9041aa0959b6" />


# TEST 3: Main Router BGP Peering : 

```show ip bgp summary```

Expected:
```text
Neighbor        V    AS  State/PfxRcd
200.1.1.2       4  65001      1
```
What we're testing: BGP session established, learning 1 route (8.8.8.8)

<img width="791" height="405" alt="image" src="https://github.com/user-attachments/assets/692a30bd-10e1-4528-bbae-e5e4c48afff3" />

# TEST 4: Main Router OSPF Neighbors : 

``` show ip ospf neighbor ``` 

Expected: 4 neighbors (one from each building)
```
Neighbor ID    Pri   State     Address         Interface
2.2.2.2          0   FULL/    10.0.10.2       Se0/3/0
3.3.3.3          0   FULL/    10.0.10.6       Se0/3/1
4.4.4.4          0   FULL/    10.0.10.10      Se0/2/0
5.5.5.5          0   FULL/    10.0.10.14      Se0/1/0
```
What we're testing: OSPF adjacency with all 4 building routers

<img width="791" height="421" alt="image" src="https://github.com/user-attachments/assets/a222056f-81c7-4a88-8a9c-734a5b6e00f0" />

# TEST 5: Main Router NAT Verification : 

```show ip nat translations```

Wait for: A PC to ping 8.8.8.8 first
Expected:
```text
Pro  Inside global    Inside local   Outside local  Outside global
icmp 200.1.1.1:1234   10.0.0.15:1234  8.8.8.8:1234   8.8.8.8:1234
```
What we're testing: NAT is translating private to public IPs




# CS BUILDING TESTS : 

### CS Router 
```
show ip interface brief | include 0/0
```

Expected:
```text
G0/0.10        10.0.0.1        YES manual up
G0/0.11        10.0.0.129      YES manual up
G0/0.12        10.0.0.193      YES manual up
G0/0.99        10.0.254.1      YES manual up
```
What we're testing: All sub-interfaces are up (Router-on-a-Stick working)

<img width="791" height="421" alt="image" src="https://github.com/user-attachments/assets/e7be9611-e70b-49b8-bdfd-3a9f269d27b7" />

### CS Router DHCP Pools :

``` show ip dhcp pool ```

Expected: 3 pools active
```text
Pool CS-LABS :
Pool CS-FACULTY :
Pool CS-TAS :
```
<img width="803" height="615" alt="image" src="https://github.com/user-attachments/assets/8e94c94d-c1a1-4a2c-8c16-d23f9dfd0291" />

### CS Distribution Switch VLANs : 

```show vlan brief```
Expected:
```text
VLAN 10   CS-LABS      active
VLAN 11   CS-FACULTY   active
VLAN 12   CS-TAS       active
VLAN 99   MGMT-CS      active
```
What we're testing: All VLANs created

<img width="794" height="466" alt="image" src="https://github.com/user-attachments/assets/589f5ee9-8870-448b-8faf-46f51c058003" />

### CS Distribution Switch Trunks : 

``` show interface trunk ```
Expected: 4 trunk ports (1 to router, 3 to access switches)
```text
Port        Mode         Status
Gi1/0/1     on           trunking
Gi1/0/2     on           trunking
Gi1/0/3     on           trunking
Gi1/0/4     on           trunking
```

<img width="805" height="783" alt="image" src="https://github.com/user-attachments/assets/efbde692-d942-4ad2-a6a1-1669287b0535" />

###  CS Access Switch 1 (Labs) : 
Check VLAN assignment
```cisco
show vlan id 10
```
 Expected: Ports Fa0/1-24 in VLAN 10

<img width="813" height="431" alt="image" src="https://github.com/user-attachments/assets/3581dcbc-d034-4b17-bdb1-efae44253045" />

### Check port security
```cisco
show port-security
```
Expected: 24 ports with "2" max addresses

<img width="794" height="524" alt="image" src="https://github.com/user-attachments/assets/1eb8007f-2bbb-4e75-a8d0-04cacfe013f2" />

### Ping management
```cisco
ping 10.0.254.2
```
 Expected: Reply from Distribution Switch

 <img width="792" height="289" alt="image" src="https://github.com/user-attachments/assets/509b13b0-86a5-4cc9-98ea-ca694defa713" />

### DHCP : 
<img width="799" height="977" alt="image" src="https://github.com/user-attachments/assets/a25c52e8-cd5b-43d6-acd6-b19ea38390bc" />



