
# Network Services & Business Continuity

## Project Overview
This project involved configuring two Windows Server 2022 machines to provide reliable DHCP services through a Hot Standby failover relationship. The goal was to improve network availability and maintain essential services if the primary DHCP server became unavailable.

## Lab Environment
- Windows Server 2022
- ZYWIN01 (Primary DHCP Server)
- ZYWIN02 (Standby DHCP Server)
- DHCP Server Role
- DHCP Management Console

## Tasks Completed

### 1. DHCP Server Installation
- Installed the DHCP Server role on ZYWIN01.
- Completed the DHCP post-installation configuration.
- Installed the DHCP Server role on ZYWIN02.

### 2. DHCP Scope Configuration
Created a DHCP scope named LAN on ZYWIN01 with the following settings:

| Parameter | Configuration |
|---|---|
| Scope Name | LAN |
| IP Address Range | 192.168.10.2 – 192.168.10.202 |
| Subnet Mask | 255.255.255.0 |
| Exclusion Range | 192.168.10.100 – 192.168.10.104 |
| Default Gateway | 192.168.10.1 |
| Lease Duration | 7 Days |
| Parent Domain | mycompany.com |

### 3. DHCP Failover Configuration
Configured a DHCP failover relationship between both servers.

- Primary Server: ZYWIN01
- Partner Server: ZYWIN02
- Failover Mode: Hot Standby
- Partner Role: Standby
- Message Authentication: Disabled

### 4. Verification
Reviewed the DHCP scope and failover configuration in the DHCP Management Console.

## Results
Successfully installed and configured DHCP services on two Windows Server machines and established a Hot Standby failover relationship to support network availability and business continuity.

## Skills Demonstrated
- Windows Server Administration
- DHCP Installation and Configuration
- IP Address Management
- Network Configuration
- DHCP Failover
- High Availability
- Business Continuity Planning

## Environment Disclaimer
This project was completed in a virtual lab environment for educational and portfolio purposes.
