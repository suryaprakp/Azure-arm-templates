This template is a conditional template which deploys Citrix SD-WAN virtual machines in highly available/ Stand alone mode.This template deploys following things 

In case of HA mode, This template creates:
- 2 SD-WAN vm's with 4 subnets for management,LAN,WAN,AUX
- UI associated with Azure portal ( createUidefinition )
- Availability set for HA 
- External LB ( Standard SKU ) - WAN endpoint to the internet
- Internal LB ( Standard SKU ) - LAN gateway internal to VNET
- IP Forwarding enabled to intercept packets not destined to adapter
- VM's with managed disks
- SKU specific VM including per hour licensing
- Security groups associated with adapters depending on the traffic patterns

In case of Standalone mode, This template creates:
- 1 SD-WAN vm with 3 subnet for management,LAN,WAN
- UI associated with Azure portal ( createUidefinition )
- VM with managed disk
- Gateway deployment in VNET
- IP Forwarding enabled to intercept packets not destined to adapter
- SKU specific VM including per hour licensing
- Security groups associated with adapters depending on the traffic patterns
