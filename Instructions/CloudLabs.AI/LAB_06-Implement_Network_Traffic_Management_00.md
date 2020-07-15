---
lab:
    title: '06 - Implement Traffic Management'
    module: 'Module 06 - Network Traffic Management'
---

# Lab 06 - Implement Traffic Management
# Student lab manual

## Lab scenario

You were tasked with testing managing network traffic targeting Azure virtual machines in the hub and spoke network topology, which Contoso considers implementing in its Azure environment (instead of creating the mesh topology, which you tested in the previous lab). This testing needs to include implementing connectivity between spokes by relying on user defined routes that force traffic to flow via the hub, as well as traffic distribution across virtual machines by using layer 4 and layer 7 load balancers. For this purpose, you intend to use Azure Load Balancer (layer 4) and Azure Application Gateway (layer 7).

## Objectives

In this lab, you will:

+ Task 1: Provision the lab environment
+ Task 2: Configure the hub and spoke network topology
+ Task 3: Test transitivity of virtual network peering
+ Task 4: Configure routing in the hub and spoke topology
+ Task 5: Implement Azure Load Balancer
+ Task 6: Implement Azure Application Gateway

## Estimated timing: 60 minutes

## Instructions

