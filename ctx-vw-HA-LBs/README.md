This template deploys Citrix SD-WAN virtual machines in a highly available/ Stand alone mode.This template deploys following things 
<ul>
<li>Its a conditional template taking care of both HA as well as normal deployment</li>
<li>In case of HA , This template creates</li>
<li>In case of standalone deployment, This template creates</li>
</ul>
   
   a) 2 SD-WAN vm's with 4 subnets for management,LAN,WAN,AUX
   b) UI associated with Azure portal ( createUidefinition )
   c) Availability set for HA 
   d) External LB ( Standard SKU ) - WAN endpoint to the internet
   e) Internal LB ( Standard SKU ) - LAN gateway internal to VNET
   f) SKU specific VM including per hour licensing
   g) VM's with managed disks
   h) Security groups associated with adapters depending on the traffic patterns

 
   

   a) 1 SD-WAN vm with 3 subnet for management,LAN,WAN
   b) UI associated with Azure portal ( createUidefinition )
   c) VM with managed disk
   d) SKU specific VM including per hour licensing
   e) Gateway deployment in VNET
   f) Security groups associated with adapters depending on the traffic patterns
