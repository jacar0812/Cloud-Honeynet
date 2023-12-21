# Building a Honeynet + SOC in Azure 
![image](https://github.com/jacar0812/Cloud-Honeynet/assets/129025552/34353cc1-dd3d-4725-bb53-45095447dfda)


## Introduction

In this project, I built a miniature honeynet infrastructure within Microsoft Azure. This involved orchestrating a simulated network environment aimed at attracting and monitoring potential cyber threats. I ensured the ingestion of diverse log sources, from various endpoints, into a centralized Log Analytics Workspace. 

The architecture of the mini honeynet in Azure consists of the following components:

- Virtual Network (VNet) 
- Network Security Group (NSG)
- Virtual Machines (2 Windows (one is used as an ATTACK-VM), 1 Linux)
- Log Analytics Workspace
- Azure Key Vault
- Azure Storage Account
- Microsoft Sentinel

The Network Security Group (Layer 4 Firewall) for both VMs was configured to allow **ALL** inbound traffic.  By deliberately allowing all inbound traffic to the Virtual Machines (VMs) in the Network Security Group (NSG), I created an environment where I could observe and study a wide range of attacks. This could include port scanning, brute-force attempts, malware propagation, and more, providing valuable insights into how attackers operate and allowing for the development of better defense mechanisms and incident response strategies.

## Conclusion

In this project, a mini honeynet was constructed in Microsoft Azure, and log sources were integrated into a Log Analytics workspace. Microsoft Sentinel was employed to trigger alerts and create incidents based on the ingested logs. 
