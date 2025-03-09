# Azure VNet Deployment with Security & DNS

## Overview
This project demonstrates how to deploy a secure Azure Virtual Network (VNet) using ARM Templates. The deployment includes:
- Automated creation of a VNet (`ManufacturingVnet`) with subnets.
- Implementation of Network Security Groups (NSG) and Application Security Groups (ASG).
- Configuration of inbound and outbound security rules.
- Public and Private DNS setup for name resolution.

## Deployment Files
| File Name | Description |
|-----------|-------------|
| `ManufacturingVnet-template.json` | ARM Template for VNet Deployment |
| `ManufacturingVnet-parameters.json` | Parameters for flexible deployment |
| `NSG-Rules.md` | Documentation for NSG & ASG Security Rules |
| `DNS-Configuration.md` | Details on Public & Private DNS setup |

## How to Deploy
1. Clone this repository:
