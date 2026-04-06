Multi-Site Network Lab
About the Project
Simulated an enterprise network in Cisco Packet Tracer featuring a headquarters and branch office connected over a WAN link using a serial connection with a /30 subnet.

What I Built
🏢 HQ — R1 + SW1

Created VLANs 10, 20, and 30 for Management, IT, and Staff
Configured the port facing R1 on SW1 as a trunk and allowed VLANs 10, 20, and 30
Configured access ports on SW1 for each end host and assigned them to their correct VLAN
Created subinterfaces on R1 for each VLAN and assigned the first available IP from each subnet as the default gateway

🏬 Branch — R2 + SW2

Created VLANs 40 and 50 for Staff and Guest
Configured the port facing R2 on SW2 as a trunk and allowed VLANs 40 and 50
Created subinterfaces on R2 for each VLAN with the correct IP addresses

🔁 Routing

Configured OSPF process ID 1 area 0 on both routers and advertised all connected subnets including the WAN link
Verified neighbor relationships were fully established before testing
Confirmed end-to-end connectivity by pinging from PC1 (VLAN 10) to all PCs across all VLANs, including across the WAN link


🛠️ Tools Used
ToolPurposeCisco Packet TracerNetwork simulationGoogle SheetsIPAM documentation

📁 Files in This Repo
PathDescription/screenshotsshow vlan brief, show interfaces trunk, show ip route, and ping verification outputs/configsFull running configurations for R1, R2, SW1, and SW2Network-Lab-IPAM.xlsxFull IP address management spreadsheet documenting every device, interface, subnet, VLAN, and role
