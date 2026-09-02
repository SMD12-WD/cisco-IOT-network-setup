# Cisco IoT Network & Security Simulation

Designed and configured a segmented IoT network in **Cisco Packet Tracer**, implementing VLANs, inter-VLAN routing, DHCP, wireless connectivity, network services, and security controls.

### What I Implemented

* **VLAN Segmentation:** Created separate VLANs to isolate departments, servers, and IoT devices, improving network organisation and reducing unnecessary communication between network segments.
* **Inter-VLAN Routing:** Configured router subinterfaces to enable controlled communication between VLANs using 802.1Q trunking.
* **DHCP:** Configured DHCP pools for different VLANs, providing devices with automatic IP addressing, default gateways, and DNS server information.
* **Wireless IoT Connectivity:** Connected IoT devices through a Wireless Access Point (WAP) and integrated the wireless IoT network into the wider network infrastructure.
* **Network Services:** Configured services including DNS, DHCP, HTTP/HTTPS, FTP, and email using a network server.
* **Extended ACLs:** Implemented an extended access control list named `IOT-SECURITY` to control traffic originating from the IoT VLAN.
* **IoT Security Controls:** Used ACL rules to block:

  * Telnet (TCP 23) to prevent insecure remote management.
  * HTTP (TCP 80) from IoT devices.
  * HTTPS (TCP 443) from IoT devices as part of the security simulation.
  * Communication between the IoT VLAN and Guest VLAN.
* **ACL Verification:** Used Cisco IOS commands such as `show access-lists`, `show ip interface`, and `show ip interface brief` to verify ACL configuration, placement, and traffic matches.

### Security Objective

The project demonstrates how **network segmentation and access control** can be used to reduce the attack surface of an IoT environment. IoT devices were separated from other network segments and restrictions were placed on potentially unnecessary or insecure traffic.


