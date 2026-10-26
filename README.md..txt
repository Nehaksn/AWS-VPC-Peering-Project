 AWS VPC Peering Project

 1. Project Overview
This project demonstrates private network communication between two Amazon EC2 instances using AWS VPC Peering.

2. Objectives
- Configure two Virtual Private Clouds (VPCs).
- Establish a VPC peering connection.
- Configure route tables for communication between the VPCs.
- Configure security rules to permit required traffic.
- Verify connectivity using ICMP ping.

 3. AWS Services Used
- Amazon VPC
- Amazon EC2
- VPC Peering
- Route Tables
- Security Groups
- Network ACLs
- Amazon Linux 2023

 4. EC2 Instance Details

| Instance | Private IP |
|---|---|
| ewb-ec2-a | 10.10.1.102 |
| ewb-ec2-b | 172.31.15.75 |

 5. Implementation Summary
1. Launched two EC2 instances.
2. Configured VPC peering between the VPCs.
3. Configured routing and network access.
4. Connected to the instances using EC2 Instance Connect.
5. Tested communication between the instances using private IP addresses.

 6. Connectivity Testing

 Test 1: EC2-A to EC2-B
Command:

ping -c 4 172.31.15.75`

Result: 4 packets transmitted, 4 received, 0% packet loss.

 Test 2: EC2-B to EC2-A
Command:

ping -c 4 10.10.1.102`

Result: 4 packets transmitted, 4 received, 0% packet loss.

Both tests successfully demonstrated communication between the two EC2 instances.

 7. Screenshots
The `screenshots/` directory contains evidence of:
- EC2 instances and their status
- VPC details
- VPC peering connection
- Route table configuration
- Successful ping from EC2-A to EC2-B
- Successful ping from EC2-B to EC2-A

 8. Conclusion
The project demonstrated successful private-IP communication between two EC2 instances through the configured AWS networking environment.

 9. Author
Neha K Swaminathan