## OSPF Transition

### R1 Configuration Changes:
- **Added OSPF Configuration:**
  - `router ospf 1`
  - `network 10.10.10.0 0.0.0.255 area 0`
  - `network 10.10.30.0 0.0.0.255 area 0`
  - `network 1.1.1.0 0.0.0.255 area 0`
- **Removed Static Route:**
  - `no ip route 20.20.20.0 255.255.255.0 1.1.1.2`

### R2 Configuration Changes:
- **Added OSPF Configuration:**
  - `router ospf 1`
  - `network 20.20.20.0 0.0.0.255 area 0`
  - `network 1.1.1.0 0.0.0.255 area 0`
- **Removed Static Route:**
  - `no ip route 10.10.10.0 255.255.255.0 1.1.1.1`

### Connectivity Issue:
- Ping from R2 to PC1 and PC2 failed, indicating a potential issue with OSPF or network connectivity.