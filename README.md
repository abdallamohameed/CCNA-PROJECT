# CCNA-PROJECT
🌐 CCNA Enterprise Network Simulation Project
      📌 Overview
          This project demonstrates the design and implementation of a small-to-medium enterprise network using Cisco technologies in Packet Tracer.
          The lab integrates Switching, Routing, Security, Network Services, and WAN technologies to simulate a real-world production environment following CCNA-level best practices.
          The objective is to build a scalable, segmented, secure, and dynamically routed network that supports multiple departments, centralized services, and secure authentication.
          
🏗️ Network Architecture

The topology is divided into multiple logical areas:

🔹 Access Layer

    End devices (PCs, Laptops, WiFi users)
    VLAN segmentation per department
    Access switches
    DHCP clients
    
🔹 Distribution Layer

    Inter-VLAN Routing
    Policy enforcement (ACLs)
    DHCP services
    Security controls

🔹 Core/WAN Layer

    3 Routers connected with EIGRP
    Serial link for default routing
    External connectivity simulation

🔹 Server Farm

    Centralized services:
      DNS Server
      Web Server
      Mail Server
      RADIUS Authentication Server

🎯 Project Goals

    The network was designed to achieve:

      ✅ Logical segmentation using VLANs
      ✅ Controlled inter-VLAN communication
      ✅ Automatic IP addressing using DHCP
      ✅ Dynamic routing with EIGRP
      ✅ Centralized AAA authentication
      ✅ Traffic filtering with ACLs
      ✅ Redundancy using EtherChannel
      ✅ Loop prevention using Rapid STP
      ✅ DHCP attack prevention with Snooping
      ✅ Route redistribution between protocols
      ✅ Secure remote access using SSH only

🔧 Implemented Technologies
  🔹 Switching

      VLAN segmentation
      Access & trunk ports
      Rapid-PVST
      EtherChannel (LACP)
      DHCP Snooping with trusted ports

  🔹 Routing

      Router-on-a-Stick for inter-VLAN routing
      EIGRP dynamic routing between routers
      Default route via serial connection
      Static route redistribution into EIGRP

  🔹 Network Services

      DHCP pools for all VLANs
      Central DNS configuration
      Central server farm
      Automated client addressing

  🔹 Security

      SSH-only remote access
      Encrypted passwords
      Local + RADIUS AAA authentication
      Extended ACLs for traffic filtering
      DHCP Snooping to prevent rogue servers

  🔐 Security Policies

      The following controls were enforced:
      Access Restrictions
      Specific host blocked from DNS usage
      Certain VLAN restricted from Web access
      VLAN 10 prevented from Mail services
      Device Security
      Password encryption enabled
      SSH instead of Telnet
      Centralized login authentication via RADIUS
      Infrastructure Protection
      STP loop prevention
      EtherChannel redundancy
      DHCP Snooping trusted uplinks

  🌍 Dynamic Routing Strategy
      Protocol Used
      
      EIGRP
      Benefits
      Fast convergence
      Automatic neighbor discovery
      Efficient bandwidth usage
      Supports route redistribution
      Suitable for enterprise scale

  📡 Redundancy & High Availability

      The design includes:
      EtherChannel aggregated links
      Rapid Spanning Tree
      Multiple router paths
      Dynamic route recalculation
      Centralized services

  🖥️ Server Roles

      Server	Purpose
      DNS	Name resolution
      Web	HTTP services
      Mail	SMTP services
      RADIUS	AAA authentication
      
  🚀 Skills Demonstrated

      This project demonstrates practical knowledge of:
      Cisco Switching
      VLAN Design
      Inter-VLAN Routing
      Dynamic Routing Protocols
      Network Security (ACL/AAA)
      Enterprise DHCP Design
      Redundancy & High Availability
      Troubleshooting methodologies

  📘 Conclusion

    This lab simulates a realistic enterprise network and integrates multiple CCNA domains into a single scalable architecture.
    It focuses on segmentation, automation, security, and reliability, which are core principles of modern network design.
    
    The project provides hands-on experience equivalent to real-world deployment scenarios and serves as a strong foundation for CCNA/CCNP-level networking.
