# Notes 05: Networking & Content Delivery

•	**Computer network:** two or more machines connected to communicate and that can be partitioned into subnets. 

•	Machines within the network carries a personal IP address which is expressed by four decimal number separated by dots and 
these numbers represent bits. (0 to 255) 

•	IPv4 is 32-bit and IPv6 address is 128-bit. 

**Open System** Interconnection model is used to understand where communication takes place. 
Amazon VPC

•	Allows the user to access an isolated section within AWS Cloud where one may launch resources in a user defined virtual network. 

     o	Selection of IP address range 

    o	Subnets such as private and public; belong to single availability zones 

    o	Configuration of route tables and networking resources

•	Use multiple layers of security and customize network configuration

•	Belongs to a single AWS Region spanning of many Availability Zones 

•	Assign the VPC an IPv4 CIDR Block & cannot change address range after creation, no overlapping

•	Public IPv4 address is manually assigned through Elastic IP address and auto assigned through public IP address settings at subnet level 

•	Elastic IP address is associated with AWS account, can be remapped, can have additional costs

•	Elastic network Interface is a virtual network interface that can attach and detach to and from an instance and attached to another instance to redirect network. 

**Route tables and routes:** 

    o	Route table contains rules that can direct network traffic from subnets 

    o	Each route specified destination 

    o	Every route table contains a local route for communication 

    o	Every subnet must be associated with a route table. 

**VPC Networking Options:** 

•	Internet Gateway allows communication between instances within VPC and public internet. 

    o	Provide a target in VPC route tables for internet traffic

   o	Perform network address translation for instances with IPv4 addresses 

•	NAT or network address translation enables private instances to be connected into the internet, but public users will not be able to connect. 

**VPC sharing** allows users to share subnets with other accounts in same organization.

   o	Enables AWS accounts to create application resources 

**VPC peering** connection allows users to privately route traffic between two VPC 

   o	Instances in different VPC can communicate as if they were on the same network 

    o	Connection between VPC’s in other AWS accounts and in other AWS regions is possible 

**AWS Direct Connect** allows users to establish dedicated private connection between network and locations 
VPC Security 

•	Security Group acts as a virtual firewall that has control over inbound outbound traffic within instance. 

    o	You can assign each instance within VPC to a different set of security groups 

•	Network access control list control traffic in and out of subnet 

    o	Set up network ACL’s with rules as ACL’s is always needed 

    o	Specify ports and protocols 

    o	Associate network ACL with multiple subnets but subnets can only have one ACL 

**Amazon Route 53**

“Domain Name System (DNS) it functions like a phone book where internet names are replaced for the IP addresses of corresponding machines.”

Amazon CloudFront 

“Amazon CloudFront is a fast content delivery service that securely delivers data to customers at high transfer speeds and it also provides a developer friendly environment.”

Questions: None
