### Step 3: Network and VPC Configuration

#### VPC Creation
Created `MySecureVPC` with a CIDR block of `10.0.0.0/16`.

#### Subnet Configuration
- **Public Subnet**: `10.0.1.0/24` with auto-assigned public IPs enabled.
- **Private Subnet**: `10.0.2.0/24` with no public IPs assigned.

#### Internet Gateway and Routing
Attached an Internet Gateway to `MySecureVPC` and set up a route for public internet access for the Public Subnet.

#### Security Groups
- **PublicSG**: Allowed HTTP, HTTPS, and SSH for instances in the Public Subnet.
- **PrivateSG**: Allowed traffic only from the PublicSG

