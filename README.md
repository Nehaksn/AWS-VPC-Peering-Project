AWS VPC Peering Project

Project Overview
This project demonstrates private network communication between two Amazon EC2 instances using AWS VPC Peering.

 Objectives
- Configure two Virtual Private Clouds (VPCs).
- Establish a VPC peering connection.
- Configure route tables.
- Configure security groups to allow required traffic.
- Test connectivity using ping.

 AWS Services Used
- Amazon VPC
- Amazon EC2
- VPC Peering
- Route Tables
- Security Groups
- Network ACLs
- Amazon Linux 2023

 EC2 Instance Details

| Instance | Private IP |
|---|---|
| ewb-ec2-a | 10.10.1.102 |
| ewb-ec2-b | 172.31.15.75 |

Implementation
1. Launched two EC2 instances.
2. Configured VPC peering.
3. Configured routes and network access.
4. Connected to the instances using EC2 Instance Connect.
5. Tested connectivity using private IP addresses.

Connectivity Test Results

 EC2-A to EC2-B
Command: `ping -c 4 172.31.15.75`

Result: 4 packets transmitted, 4 received, 0% packet loss.

 EC2-B to EC2-A
Command: `ping -c 4 10.10.1.102`

Result: 4 packets transmitted, 4 received, 0% packet loss.

 Screenshots
Screenshots of the EC2 instances, VPC configuration, peering connection, route tables, and connectivity tests are included in this repository.

Conclusion
Both EC2 instances successfully communicated using their private IP addresses in the configured AWS networking environment.

Author
Neha K Swaminathan
