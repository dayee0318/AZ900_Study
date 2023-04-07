#AZ900: Azure Fundamentals

## Cloud Computing
- lets you choose the power and features you need to run your software.
- Pay for only the services you use
- Someone else manage the upkeep of the computer

### Computer Power
- Main service that cloud computing provides (computing service)
- How much processing your computer can do (=RAM)
- Cloud computing allows users to add/remove computer power as you need it (=cost save)

### Storage
- Service component of cloud computing
- Volume of data (=Hard Drive Space)
- Backups, OS up to date, Up and running for 24-hour a day.

## Shared responsibility model
- Saas: Software as a service
- Paas: Platform as a service
- Iaas: Infrastructure as a service

C: Customer responsibility  
M: Microsoft responsibility  
S: Shared responsibility   

|**Responsibility** | **Saas** | **Paas** | **Iaas** |
|----------------|------|------|------|
|Information and data | C | C | C |
Devices | C | C | C | C |
Accounts and identities | C | C | C |
Identity and directory infrastructure | S | S | C |
Applications | M | S | C |
Network controls | M | S | C |
Operating system | M | M | C |
Physical hosts | M | M | M |
Physical network | M | M | M |
Physical datacenter | M | M | M |


- Always customer's responsible for:
  - The information and data stored in the cloud
  - Devices that are allowed to connect to the cloud
  - Accounts and identities of the people, services, and devices within the organization


- Always Cloud provider's responsible for:
  - The physical datacenter
  - The physical network
  - The physical hosts


- Customer's responsibility:
  - Iaas > Paas > Saas


## Cloud models
- deployment type of cloud resources.

### Private cloud
- Natural evolution from a corporate datacenter.
- Used by a single entity
- Provides much greater control for the company
- Greater cost & fewer benefit

#### ↕ difference: general public availiability

### Public cloud
- Built, controlled, and maintained by a third-party cloud provider

### Hybrid cloud
- uses both public & private cloud in an inter-connected environment

public cloud | private cloud | Hybrid cloud
-------------|---------------|-------------
No capital expenditures to scale up | Organizations have complete control over resources and security | Provides the most flexibility
Applications can be quickly provisioned and deprovisioned | Data is not collocated with other organizations' data | Organizations determine whtere to run their applications
Organizations pay only for what they use | Hardware must be purchased for startup and maintenance | Organizations control security, compliance, or legal requirements
Organizations don't have complete control over resources and security | Organizations are responsible for hardware maintenance and updates

### Multi-cloud
- Use multiple **public** cloud providers.
- use different features from different cloud providers
- Started using a cloud service, and are in process of migrating to a different provider.
- = Deal with 2+ public cloud providers and manage resources and security in both environment.

### Azure Arc
- Set of technologies that helps manage cloud environment.

### Azure VMware Solution
- Lets you run your VMware workloads in Azure with seamless integration and scalability.

## Consumption-based model
### Capital expenditure (CapEx)
- one-time, up-front expenditure to purchase or secure tangible resources
- (Ex: new building, repaving parking lot, building a datacenter)

### Operational expenditure (OpEx)
- spending money on services or products over time
- (Ex: renting a convention center, leasing a car, **sign up for cloud services**)

### Cloud computing is OpEx
- Pay for IT resources you use → consumption-based model
- No upfront costs
- No need to purchase & manage costly infrastructure that users might not use
- The ability to pay for more resources when they're needed.
- The ability to stop paying for resources that are no longer needed.
