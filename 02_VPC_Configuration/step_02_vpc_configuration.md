### Step 3: Network and VPC Configuration
![image](https://github.com/user-attachments/assets/36b1de67-e6f9-4ac9-a9e4-c532d39941f5)


#### VPC Creation
Created `MySecureVPC` with a CIDR block of `10.0.0.0/16`.
![image](https://github.com/user-attachments/assets/0882e7b1-3336-4e28-b8ff-fc5f59eadc37)


#### Subnet Configuration
- **Public Subnet**: `10.0.1.0/24` with auto-assigned public IPs enabled.
- **Private Subnet**: `10.0.2.0/24` with no public IPs assigned.

#### Internet Gateway and Routing
Attached an Internet Gateway to `MySecureVPC` and set up a route for public internet access for the Public Subnet.

#### Security Groups
- **PublicSG**: Allowed HTTP, HTTPS, and SSH for instances in the Public Subnet.
- **PrivateSG**: Allowed traffic only from the PublicSG

