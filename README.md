# IAC-Diagram-Coporate-only-cloud

Extension of the on-premises network

In this case, you’d have a network that only contains private subnets, and does not have NAT Gateways. These components get replaced by a VGW (Virtual Gateway) and a VPN Connection. You’ll also need a CGW (Customer Gateway), which represents the on-premises side of the VPN Connection.

### STEP 1 ###

In the lucid blank page, choose AWS container. 

### STEP 2 ###

Inside the AWS Container, create a VPC (Virtual Private Cloud) container. 

### STEP 3 ###

Inside the VPC Container, create two AZ (Avalibility Zones). This is done two help with resilence and high avalibilty.

### STEP 4 ###

Inside the AZ's, create Private Subnets in each of the AZ's. 

### STEP 5 ### 

Create a Virtual Private Gateway on the edge of the VPC Container. 

### STEP 6 ### 

Connect a VPN Connection or Tunnel. The VPN sits outside the cloud. This is done only to secure connection only between the VPN and the gateway. 

### STEP 7 ###

The VPN is connected to the Customer gateway. The Customer gateway is connected to the On-prem Data center. 
