# MPLS

## Environment:
### Platform: GNS3
### Routers: IOU L3 devices

## Project Overview:
This MPLS lab setup is designed to provide hands-on experience with end-to-end MPLS configurations. It's focused on building connectivity between customer sites using different VRFs and peering setups.

### Initial Configurations:
The initial configuration files contain the startup configuration for all nodes. Each configuration is clearly marked with its respective hostname. You'll find this under the folder named initial_configs.

### Project Goals:
End-to-End Connectivity: The primary goal of this lab is to ensure that end-to-end connectivity exists between the customer sites.
Peering: No initial peering configurations between customer sites are provided in the initial configurations. Therefore, you have the freedom to choose which customer edges (CEs) you'd like to peer.
VRF Nomencalture: Naming of VRFs is left open. However, in the provided solution (after_configs folder), you'll find that CE1 is peered with CE3, and CE2 is peered with CE4. The chosen VRFs for this solution are Customer_A and Customer_B.
Routing Protocol: Choose your preferred routing protocol for peering between CEs and PEs. In the provided solution, eBGP was chosen. For your convenience, loopback interfaces on CE1-4 are set to 1.1.1.1, 2.2.2.2, 3.3.3.3, and 4.4.4.4 respectively.
ISP Core Configuration: The ISP core, consisting of routers R1-12, is pre-configured to run OSPF process 1. This allows you to focus mainly on the CEs and PEs configurations.

### Completion Checks:
Once you've finished the lab setup, ensure that:

Each VRF on the customer edges has end-to-end routes.
If you chose to configure loopback interfaces, you should be able to ping the loopback interface of one customer site from the other within the same VRF.
### Usage:
Anyone interested in utilizing this MPLS lab setup is welcome to do so. Feel free to clone the repository, make modifications, and test different configurations to your heart's content.

### Contribution:
If you've made any improvements or found any issues, kindly raise a pull request or an issue respectively. Your contributions will be appreciated.


