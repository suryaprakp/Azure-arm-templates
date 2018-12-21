This template deploys Citrix Wanopt virtual machine in Stand alone mode.This template deploys following things 

In case of Standalone mode, This template creates:
- 1 WANopt vm with 1 subnet for management 
- UI associated with Azure portal ( createUidefinition )
- VM with managed disk
- one-arm deployment in VNET
- IP Forwarding enabled to intercept packets not destined to adapter
- Security groups associated with adapters depending on the traffic patterns
