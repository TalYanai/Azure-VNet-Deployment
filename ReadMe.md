# Network Setup for Azure

## Overview

This project contains the setup for two Virtual Networks (VNets) in Azure, along with Peering and Route Tables to facilitate connectivity between them.

The setup is divided into three major parts:
1. **CoreInfraVnet**: First VNet setup.
2. **ProdInfraVnet**: Second VNet setup.
3. **Peering and Routes**: Peering between the two VNets and routing configuration.

## JSON Templates

This project includes three JSON templates:

### 1. `CoreInfraVnet.json`
This template creates the **CoreInfraVnet** with a specified address space and subnets. The **CoreInfraVnet** is intended to be the main network used in the infrastructure.

### 2. `ProdInfraVnet.json`
This template creates the **ProdInfraVnet** with a specified address space and subnets. This network will be peered with **CoreInfraVnet** to enable inter-network communication.

### 3. `PeeringAndRoutes.json`
This template sets up **Peering** between **CoreInfraVnet** and **ProdInfraVnet**. Additionally, it configures custom **Route Tables** for traffic routing between these two networks.

## Steps to Deploy

1. Open the **Azure Portal**.
2. Create a **Resource Group**.
3. Use the following steps to deploy each JSON template:
   - Go to **Deployments** in the resource group.
   - Select **Template deployment**.
   - Upload the desired JSON template and deploy it.

## Prerequisites

- **Azure Subscription**.
- Basic knowledge of **Virtual Networks**, **Peering**, and **Route Tables**.

## Troubleshooting

If you encounter issues with the Peering or Route Tables, ensure the following:
- The VNets are in the **same region**.
- The **NSG** and **Firewalls** allow traffic between the VNets.
