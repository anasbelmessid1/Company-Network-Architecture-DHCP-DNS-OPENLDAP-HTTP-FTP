# Enterprise Network Architecture

## Project Overview
This project focuses on implementing an enterprise network architecture using Ubuntu-based virtual machines (VMs). The goal is to set up and configure various network services, including DHCP, DNS, FTP, HTTP, Email, and LDAP for centralized authentication.

## Project Contributors
- **Belmessid Anas**

Supervised by:
- **Pr. Tadist Khawla**

## Abstract
The project demonstrates the setup and configuration of essential network services to create a robust enterprise network. It involves configuring DHCP, DNS, FTP, HTTP, Email, and LDAP servers to ensure seamless network management and security.

## Acknowledgments
Special thanks to Pr. Tadist Khawla for the supervision and guidance throughout the project.

## Project Structure
1. **Environment Setup**
2. **Configure DHCP for Both Subnets**
3. **Configure DNS Server**
4. **Configure FTP Server (For Subnet 1 only)**
5. **Configure HTTP Server**
6. **Configure Email Server**
7. **Configure LDAP for Centralized Authentication**
8. **Enhancements (Security)**

## Detailed Methodology

### Environment Setup
Three Ubuntu-based VMs are used to simulate the network topology and implement the network services. The first VM acts as the main server connected to the Internet and two subnets. It is assigned three Network Interface Cards (NICs):
- One NIC for Internet connection
- One NIC for Subnet 1
- One NIC for Subnet 2

The second and third VMs are each assigned one NIC and connected to Subnet 1 and Subnet 2, respectively.

### Configure DHCP for Both Subnets
Install the DHCP server program to serve IPs to the hosts over the subnets.
```bash
apt -y install isc-dhcp-server
