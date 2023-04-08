#AZ900: Azure Fundamentals

# Module 1

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

# Module 2

## Benefits of high availability and scalability in the cloud

### High availability
- Azure is a highly available cloud environment with uptime guarantees depending on the service.
- SLAs: Service-Level Agreements
  - Formal agreement between a service provider and customer
  - Guarantees the customer a stated level of service
- Azure SLA
  - represented as a percentage, related to the service or application's availability
  - (Availability = up time) → 100% available / 100% uptime = service is always available to use
  - (Unavailability = down time) → used for required maintenance or upgrades
  - Why maintaining 100%  uptime is difficult?
    - No time for maintenance / update
    - require duplicating every single component in case one component failed
    - require those backup components to pick up the service tasks with zero interruption to the customer
  - 99% and 99.9% differences?
    - 99% can be unavailable for up to 1.6 hours/week or 7.2 hours/month (Time cumulative)
    - 99.9% can be unavailable only 10 minutes/week or 43.2 minutes/month

### Scalability
- Ability to adjust resources to meet demand.
- **Vertical scaling**
  - to add more CPUs or RAM to the virtual machine (more processing power)
- ** Horizontal scaling**
  - suddenly experienced a steep jump in demand.
  - add additional virtual machines or containers, scaling out.

## Benefits of reliability and predictability in the cloud  

### Reliability
- Ability of a system to recover from failures and continue to function.
- cloud = decentralized design → naturally supports a reliable and resilient infrastructure.

### Predictability
- can be focused on **Performance predictability** or **Cost predictability**.
- Performance
  - focuses on predicting the resources needed to deliver a positive experience for your customers.
  - Autoscaling, load balancing, high availability
- Cost
  - focuses on predicting or forecasting the cost of the cloud spend.
  - Track resource use in real time, monitor resources to ensure most efficient way of using, apply data analytics to find patterns and trends
  - use tools like to Total Cost of Ownership (TCO) or pricing calculator


## Benefits of security and governance in the cloud
- Depending on your operating model, software patches and updates may also automatically be applied, which helps with both governance and security
- Security
  - can find a cloud solution that matches security needs.
  - IaaS: provides physical resources / let you manage the os and installed software, including patches and maintenance. (Max control of security)
  - PaaS: patches and maintenance taken care of automatically
- cloud is intended as an over-the-internet delivery of IT resources
- Typically, well suited to handle things like DDoS (Distributed Denial of Service) attacks, making network more robust and secure

## Benefits of manageability in the cloud
- Two types of manageability for cloud computing: Management **of** the cloud, Management **in** the cloud
- Management of the cloud: speaks to managing your cloud resources
  - automatically scale resource deployment based on need
  - Deploy resources based on a preconfigured template, removing the need for manual configuration
  - Monitor the health of resources and automatically replace failing resources
  - Receive automatic alerts based on configured metrics, so you're aware of performance in real time
- Management in the cloud: speaks to how you're able to manage your cloud environment and resources.
  - Through a web portal
  - Using a command line interface
  - Using APIs
  - Using PowerShell
