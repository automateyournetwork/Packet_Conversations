# Junos - CVE Report

## Juniper Junos 22.1R3

### CVE-2022-22219
- **Description:** Due to the Improper Handling of an Unexpected Data Type in the processing of EVPN routes on Juniper Networks Junos OS and Junos OS Evolved, an attacker in direct control of a BGP client connected to a route reflector, or via a machine in the middle (MITM) attack, can send a specific EVPN route contained within a BGP Update, triggering a routing protocol daemon (RPD) crash, leading to a Denial of Service (DoS) condition. Continued receipt and processing of these specific EVPN routes could create a sustained Denial of Service (DoS) condition. This issue only occurs on BGP route reflectors, only within a BGP EVPN multicast environment, and only when one or more BGP clients have 'leave-sync-route-oldstyle' enabled.
- **CVSS V3.1 Score:** 5.9 (Medium)
- **Vector:** CVSS:3.1/AV:N/AC:H/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2023-22394
- **Description:** An Improper Handling of Unexpected Data Type vulnerability in the handling of SIP calls in Juniper Networks Junos OS on SRX Series and MX Series platforms allows an attacker to cause a memory leak leading to Denial of Services (DoS). This issue occurs on all MX Series platforms with MS-MPC or MS-MIC card and all SRX Series platforms where SIP ALG is enabled. Successful exploitation of this vulnerability prevents additional SIP calls and applications from succeeding. The SIP ALG needs to be enabled, either implicitly / by default or by way of configuration.
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2023-22396
- **Description:** An Uncontrolled Resource Consumption vulnerability in TCP processing on the Routing Engine (RE) of Juniper Networks Junos OS allows an unauthenticated network-based attacker to send crafted TCP packets destined to the device, resulting in an MBUF leak that ultimately leads to a Denial of Service (DoS). The system does not recover automatically and must be manually restarted to restore service. This issue occurs when crafted TCP packets are sent directly to a configured IPv4 or IPv6 interface on the device. Transit traffic will not trigger this issue.
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2023-22401
- **Description:** An Improper Validation of Array Index vulnerability in the Advanced Forwarding Toolkit Manager daemon (aftmand) of Juniper Networks Junos OS and Junos OS Evolved allows an unauthenticated, network-based attacker to cause a Denial of Service (DoS). On the PTX10008 and PTX10016 platforms running Junos OS or Junos OS Evolved, when a specific SNMP MIB is queried this will cause a PFE crash and the FPC will go offline and not automatically recover. A system restart is required to get the affected FPC in an operational state again.
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2023-22408
- **Description:** An Improper Validation of Array Index vulnerability in the SIP ALG of Juniper Networks Junos OS on SRX 5000 Series allows a network-based, unauthenticated attacker to cause a Denial of Service (DoS). When an attacker sends an SIP packets with a malformed SDP field then the SIP ALG can not process it which will lead to an FPC crash and restart. Continued receipt of these specific packets will lead to a sustained Denial of Service.
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2023-22409
- **Description:** An Unchecked Input for Loop Condition vulnerability in a NAT library of Juniper Networks Junos OS allows a local authenticated attacker with low privileges to cause a Denial of Service (DoS). When an inconsistent "deterministic NAT" configuration is present on an SRX, or MX with SPC3 and then a specific CLI command is issued the SPC will crash and restart. Repeated execution of this command will lead to a sustained DoS.
- **CVSS V3.1 Score:** 5.5 (Medium)
- **Vector:** CVSS:3.1/AV:L/AC:L/PR:L/UI:N/S:U/C:N/I:N/A:H

### CVE-2023-22415
- **Description:** An Out-of-Bounds Write vulnerability in the H.323 ALG of Juniper Networks Junos OS allows an unauthenticated, network-based attacker to cause Denial of Service (DoS). On all MX Series and SRX Series platform, when H.323 ALG is enabled and specific H.323 packets are received simultaneously, a flow processing daemon (flowd) crash will occur. Continued receipt of these specific packets will cause a sustained Denial of Service (DoS) condition.
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2023-1697
- **Description:** An Improper Handling of Missing Values vulnerability in the Packet Forwarding Engine (PFE) of Juniper Networks Junos OS allows an adjacent, unauthenticated attacker to cause a dcpfe process core and thereby a Denial of Service (DoS). Continued receipt of these specific frames will cause a sustained Denial of Service condition. This issue occurs when a specific malformed ethernet frame is received.
- **CVSS V3.1 Score:** 6.5 (Medium)
- **Vector:** CVSS:3.1/AV:A/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2023-28959
- **Description:** An Improper Check or Handling of Exceptional Conditions vulnerability in packet processing of Juniper Networks Junos OS on QFX10002 allows an unauthenticated, adjacent attacker on the local broadcast domain sending a malformed packet to the device, causing all PFEs other than the inbound PFE to wedge and to eventually restart, resulting in a Denial of Service (DoS) condition. Continued receipt and processing of this packet will create a sustained Denial of Service (DoS) condition.
- **CVSS V3.1 Score:** 6.5 (Medium)
- **Vector:** CVSS:3.1/AV:A/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2023-28962
- **Description:** An Improper Authentication vulnerability in upload-file.php, used by the J-Web component of Juniper Networks Junos OS allows an unauthenticated, network-based attacker to upload arbitrary files to temporary folders on the device.
- **CVSS V3.1 Score:** 5.3 (Medium)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:L/A:N

## Juniper Junos 21.3R1

### CVE-2022-22168
- **Description:** An Improper Validation of Specified Type of Input vulnerability in the kernel of Juniper Networks Junos OS allows an unauthenticated adjacent attacker to trigger a Missing Release of Memory after Effective Lifetime vulnerability. Continued exploitation of this vulnerability will eventually lead to an FPC reboot and thereby a Denial of Service (DoS).
- **CVSS V3.1 Score:** 6.5 (Medium)
- **Vector:** CVSS:3.1/AV:A/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2022-22171
- **Description:** An Improper Check for Unusual or Exceptional Conditions vulnerability in the Packet Forwarding Engine (PFE) of Juniper Networks Junos OS allows an unauthenticated networked attacker to cause a Denial of Service (DoS) by sending specific packets over VXLAN which cause the PFE to reset.
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2022-22175
- **Description:** An Improper Locking vulnerability in the SIP ALG of Juniper Networks Junos OS on MX Series and SRX Series allows an unauthenticated networked attacker to cause a flowprocessing daemon (flowd) crash and thereby a Denial of Service (DoS). Continued receipt of these specific packets will cause a sustained Denial of Service condition.
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2022-22179
- **Description:** A Improper Validation of Specified Index, Position, or Offset in Input vulnerability in the Juniper DHCP daemon (jdhcpd) of Juniper Networks Junos OS allows an adjacent unauthenticated attacker to cause a crash of jdhcpd and thereby a Denial of Service (DoS).
- **CVSS V3.1 Score:** 6.5 (Medium)
- **Vector:** CVSS:3.1/AV:A/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2022-22180
- **Description:** An Improper Check for Unusual or Exceptional Conditions vulnerability in the processing of specific IPv6 packets on certain EX Series devices may lead to exhaustion of DMA memory causing a Denial of Service (DoS).
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2022-22191
- **Description:** A Denial of Service (DoS) vulnerability in the processing of a flood of specific ARP traffic in Juniper Networks Junos OS on the EX4300 switch, sent from the local broadcast domain, may allow an unauthenticated network-adjacent attacker to trigger a PFEMAN watchdog timeout, causing the Packet Forwarding Engine (PFE) to crash and restart.
- **CVSS V3.1 Score:** 6.5 (Medium)
- **Vector:** CVSS:3.1/AV:A/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2022-22201
- **Description:** An Improper Validation of Specified Index, Position, or Offset in Input vulnerability in the Packet Forwarding Engine (PFE) of Juniper Networks Junos OS allows an unauthenticated network-based attacker to cause a Denial of Service (DoS). On SRX5000 Series with SPC3, SRX4000 Series, and vSRX, when PowerMode IPsec is configured and a malformed ESP packet matching an established IPsec tunnel is received the PFE crashes.
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2022-22205
- **Description:** A Missing Release of Memory after Effective Lifetime vulnerability in the Application Quality of Experience (appqoe) subsystem of the PFE of Juniper Networks Junos OS on SRX Series allows an unauthenticated network based attacker to cause a Denial of Service (DoS).
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2022-22219
- **Description:** Due to the Improper Handling of an Unexpected Data Type in the processing of EVPN routes on Juniper Networks Junos OS and Junos OS Evolved, an attacker in direct control of a BGP client connected to a route reflector, or via a machine in the middle (MITM) attack, can send a specific EVPN route contained within a BGP Update, triggering a routing protocol daemon (RPD) crash, leading to a Denial of Service (DoS) condition.
- **CVSS V3.1 Score:** 5.9 (Medium)
- **Vector:** CVSS:3.1/AV:N/AC:H/PR:N/UI:N/S:U/C:N/I:N/A:H

### CVE-2022-22247
- **Description:** An Improper Input Validation vulnerability in ingress TCP segment processing of Juniper Networks Junos OS Evolved allows a network-based unauthenticated attacker to send a crafted TCP segment to the device, triggering a kernel panic, leading to a Denial of Service (DoS) condition.
- **CVSS V3.1 Score:** 7.5 (High)
- **Vector:** CVSS:3.1/AV:N/AC:L/PR:N/UI:N/S:U/C:N/I:N/A:H
