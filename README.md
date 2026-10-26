# AWS VPC Peering Project

## Project Overview

This project demonstrates private communication between two AWS Virtual Private Clouds (VPCs) using a VPC Peering Connection.

A public EC2 instance acts as a bastion host, allowing controlled access to private EC2 instances.

## AWS Services Used

* Amazon VPC
* Amazon EC2
* VPC Peering
* Internet Gateway
* Route Tables
* Security Groups

## Network Architecture

### VPC 1

* VPC CIDR: `10.0.0.0/16`
* Public Subnet: `10.0.1.0/24`
* Private Subnet: `10.0.2.0/24`
* Public EC2 Instance: Bastion Host
* Private EC2 Instance: Private EC2 in VPC1

### VPC 2

* VPC CIDR: `10.1.0.0/16`
* Private Subnet: `10.1.1.0/24`
* Private EC2 Instance: Private EC2 in VPC2

## Project Features

* VPC Peering between two VPCs.
* Public and private subnet configuration.
* Route tables for private network communication.
* Bastion host for controlled administrative access.
* Security groups for traffic control.

## Testing and Validation

* Connected to the bastion host from the local laptop.
* Accessed EC2 instances using Amazon EC2 Connect.
* Successfully tested connectivity using ping requests.
* Verified communication between private instances in both VPCs using private IP addresses.

## Project Documentation

The `project-report.pdf` file contains the project report.

The `screenshots` folder contains AWS configuration and connectivity-test evidence.

## Conclusion

This project demonstrates private communication between AWS VPCs using VPC Peering, along with controlled access to private EC2 instances through a bastion host.
