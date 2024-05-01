#  MAC Flooding Attack

## Overview

This repository explores a network security scenario focusing on a company's network that was compromised by a CAM table attack. It offers valuable insights into network vulnerabilities and security practices through the lens of a real-world incident. The project includes detailed documentation and visual representations of the network structure, the attack scenario, and comparisons of network devices such as hubs and switches. This repository serves as a comprehensive learning resource for security analysts, IT professionals, and anyone interested in understanding and preventing network attacks.


## Company Network Structure:
- The company network consists of five devices connected to one switch.
- The devices include workstations, servers, and other network-connected equipment.
- There is an additional attack device in the network, which is a penetration laboratory used for testing network vulnerabilities.

## Attack Overview:
- A CAM table attack (also known as MAC flooding) occurs when an attacker floods the switch's CAM table with a large number of fake MAC addresses.
- As a result, the switch's CAM table becomes full, causing it to enter fail-open mode and broadcast all incoming traffic to all ports.
- This allows the attacker to intercept and capture sensitive data from the network.

## Attack Execution:
- The attack begins when the attacker sends a high volume of fake MAC addresses to the switch from the penetration laboratory.
- The switch's CAM table becomes overwhelmed and cannot store more MAC addresses.
- The switch then starts broadcasting traffic to all ports, enabling the attacker to capture data from the network.

## Impact on the Company:
- Sensitive data, such as customer information, financial records, and internal communications, may be intercepted by the attacker.
- Network performance may degrade due to the increased broadcast traffic.
- The attack may go undetected initially, causing prolonged exposure to data breaches.

## Mitigation Strategies:
- Implement MAC address filtering and port security features on the switch to limit the number of MAC addresses per port.
- Use intrusion detection systems (IDS) and monitoring tools to detect and respond to abnormal network traffic.
- Regularly update and patch network devices to protect against known vulnerabilities.
- Train employees on cybersecurity best practices to recognize and report potential attacks.
