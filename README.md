# Building a Honeynet + SOC in Azure 
![image](https://github.com/jacar0812/Cloud-Honeynet/assets/129025552/34353cc1-dd3d-4725-bb53-45095447dfda)


## Introduction

In this project, I built a miniature honeynet infrastructure within Microsoft Azure. This involved orchestrating a simulated network environment aimed at attracting and monitoring potential cyber threats. I ensured the ingestion of diverse log sources, from various endpoints, into a centralized Log Analytics Workspace. 

The architecture of the mini honeynet in Azure consists of the following components:

- Virtual Network (VNet) 
- Network Security Group (NSG)
- Virtual Machines (2 Windows, 1 Linux)
- Log Analytics Workspace
- Azure Key Vault
- Azure Storage Account
- Microsoft Sentinel

First, after logging into Azure and creating a subscription, I created two virtual machines (VM).  First, I created a Windows 10 Pro VM (name it windows-vm).  That VM is put under a new Resource Group that I created (named RG-Cyber-1979)


## Conclusion

In this project, a mini honeynet was constructed in Microsoft Azure, and log sources were integrated into a Log Analytics workspace. Microsoft Sentinel was employed to trigger alerts and create incidents based on the ingested logs. 
