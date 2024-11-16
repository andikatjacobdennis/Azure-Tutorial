# **Azure-Tutorial**

## **CapEx vs. OpEx**

- **CapEx (Capital Expenditure):**  
  Refers to upfront investments in physical infrastructure or assets that the business owns and depreciates over time. For example:
  - Purchasing servers, data centers, and networking hardware.
  - Used when organizations prefer long-term cost benefits.
  - Advantage: Full control over infrastructure and predictable costs.

- **OpEx (Operational Expenditure):**  
  Refers to ongoing costs for using services or products. These are regular expenses incurred to operate a business. For example:
  - Paying for cloud services on a subscription or pay-as-you-go model.
  - Used when organizations need scalability and flexibility.
  - Advantage: Lower upfront cost and better cost predictability.

Azure, like most cloud platforms, enables organizations to shift from a CapEx model to an OpEx model by offering scalable, subscription-based services.

---

## **Types of Cloud Services**

Cloud computing services are categorized into **IaaS**, **PaaS**, and **SaaS**, each addressing specific organizational needs.

### **1. IaaS (Infrastructure as a Service):**
- Provides virtualized computing resources such as virtual machines, storage, and networks.
- Ideal for businesses wanting to avoid hardware procurement and management.
- Example in Azure:  
  - **Azure Virtual Machines**: Deploy scalable VM instances.
  - **Azure Storage**: Secure and scalable storage solutions.

### **2. PaaS (Platform as a Service):**
- Provides a platform with tools and middleware to develop, deploy, and manage applications without managing the underlying infrastructure.
- Focus is on development rather than hardware management.
- Example in Azure:  
  - **Azure App Service**: Host web apps, RESTful APIs, and mobile backends.
  - **Azure Functions**: Event-driven serverless computing for running lightweight tasks.

### **3. SaaS (Software as a Service):**
- Provides software applications over the internet on a subscription basis.
- No need for installation or maintenance.
- Example in Azure:  
  - **Microsoft 365 (Office 365)**: Cloud-based productivity tools like Word, Excel, and Teams.
  - **Dynamics 365**: Integrated CRM and ERP solutions.

---

## **Types of Cloud Deployment Models**

### **1. Public Cloud:**
- Owned and operated by third-party cloud service providers, offering shared resources to multiple tenants over the internet.
- Examples:  
  - **AWS (Amazon Web Services)**  
  - **Google Cloud Platform (GCP)**  
  - **IBM Cloud**  
  - **Microsoft Azure**  

### **2. Private Cloud:**
- A dedicated cloud environment exclusively for one organization, offering greater control and customization.
- Examples:  
  - **Azure Stack**: Azure's on-premises extension for private cloud.  
  - **VMware Cloud**: Private cloud solutions leveraging VMware technology.  
  - **Red Hat OpenShift Container Platform**: A private container platform for Kubernetes-based workloads.

#### **3. Hybrid Cloud:**
- Combines private and public clouds, enabling data and applications to move between them seamlessly.
- Examples:  
  - **Azure Arc**: Extend Azure management to any infrastructure across hybrid setups.  
  - **AWS Outposts**: Extend AWS services to on-premises infrastructure.  
  - **Google Anthos**: Hybrid solution connecting on-premises environments with Google Cloud.

---

## Introduction to Azure

Microsoft Azure is a comprehensive cloud computing platform designed to help businesses and developers build, deploy, and manage applications and services. Launched in 2010, Azure provides a wide range of cloud services, including computing, analytics, storage, networking, and AI tools. It is highly scalable and secure, catering to enterprises, startups, and individual developers alike.

With Azure, you can:
- Host websites and web applications.
- Store, analyze, and retrieve data.
- Build and train machine learning models.
- Enable IoT solutions.
- Manage virtual networks and cloud-based servers.

Azure operates on a global infrastructure and offers services in various configurations, including Infrastructure as a Service (IaaS), Platform as a Service (PaaS), and Software as a Service (SaaS).

---

## Regions and Zones

## **Azure Regions**
Azure is built on a foundation of globally distributed datacenters. These datacenters are grouped into *regions*, which are geographical locations where Microsoft has established one or more datacenters. Each region is isolated to protect against regional failures and ensure redundancy.

Examples of Azure regions:
- **East US**
- **West Europe**
- **Southeast Asia**

### Key Features of Azure Regions:
1. **Scalability and Availability**: Azure allows applications to scale across multiple regions to meet user demand.
2. **Compliance**: Many Azure regions are compliant with local regulatory requirements, such as GDPR in Europe.
3. **Latency Optimization**: Users can select regions close to their customers to minimize latency.

---

### **Availability Zones**
Within a region, Azure provides *Availability Zones* to protect applications and data from datacenter failures. Availability Zones are physically separate datacenters within a region, each equipped with independent power, cooling, and networking.

#### Key Features:
- **High Availability**: Ensure application uptime by spreading resources across multiple zones.
- **Fault Isolation**: Each zone operates independently, so issues in one zone do not affect others.
- **Data Replication**: Azure replicates data across zones to enhance durability.

Availability Zones are particularly useful for critical applications requiring high resilience. Services like Azure Virtual Machines, Kubernetes, and SQL databases support zonal deployment.

---

## Paired Regions

Azure's *Paired Regions* are a feature designed for disaster recovery and data redundancy. Each Azure region is paired with another region in the same geography. For example, **East US** is paired with **West US**, and **North Europe** is paired with **West Europe**.

### Benefits of Paired Regions:
1. **Data Residency**: Paired regions ensure data remains within the same geopolitical boundary for compliance.
2. **Automatic Recovery**: During planned maintenance or outages, services are prioritized in the paired region.
3. **Reduced Downtime**: Azure schedules updates to paired regions in a staggered manner to avoid simultaneous downtime.

Paired regions are especially important for businesses that require geo-redundancy, ensuring seamless disaster recovery.

---

## Azure Services

Azure offers an extensive catalog of services spanning multiple domains. Below are some major service categories:

### **1. Compute Services**
These services provide the building blocks for running applications and workloads:
- **Azure Virtual Machines**: Create and manage virtual servers.
- **Azure Kubernetes Service (AKS)**: Deploy and manage containerized applications.
- **Azure App Service**: Host web apps, APIs, and mobile backends.

### **2. Storage Services**
Azure’s storage solutions are secure, scalable, and durable:
- **Blob Storage**: Store large amounts of unstructured data.
- **Azure Files**: Provide shared file storage.
- **Disk Storage**: Attach high-performance disks to virtual machines.

### **3. Networking Services**
Azure networking solutions help manage and secure your network:
- **Azure Virtual Network (VNet)**: Create private networks in Azure.
- **Azure Load Balancer**: Distribute incoming traffic across servers.
- **Azure DNS**: Host DNS domains and manage DNS records.

### **4. AI and Machine Learning**
Azure provides tools for developers and data scientists:
- **Azure Machine Learning**: Build, train, and deploy ML models.
- **Cognitive Services**: Add AI capabilities like speech recognition and vision analysis to applications.
- **Bot Services**: Create intelligent chatbots.

### **5. Database Services**
Azure offers multiple database solutions:
- **Azure SQL Database**: A fully managed relational database.
- **Cosmos DB**: A globally distributed NoSQL database.
- **Azure Database for MySQL/PostgreSQL**: Managed open-source database services.

### **6. Security and Identity**
Azure provides advanced security services to protect your applications and data:
- **Azure Active Directory (Azure AD)**: Manage user identities and access.
- **Azure Sentinel**: A cloud-native SIEM (Security Information and Event Management) tool.
- **Azure Key Vault**: Securely store and access sensitive information like API keys and passwords.

### **7. Analytics**
Azure offers robust analytics tools for data-driven insights:
- **Azure Synapse Analytics**: A unified platform for big data and data warehousing.
- **Power BI**: Visualize data with interactive dashboards.
- **Data Factory**: Orchestrate and automate data workflows.

### **8. Developer Tools**
Azure integrates seamlessly with developer ecosystems:
- **Azure DevOps**: Manage CI/CD pipelines.
- **Azure Functions**: Build serverless applications.
- **Azure Logic Apps**: Automate workflows and integrate with third-party systems.


---

## **1. Subscription and Account**

An **Azure Subscription** is a logical container used to provision and manage Azure resources. It associates resources with billing, access control, and organizational policies.

### Key Concepts:
- **Account**: Your Microsoft account or organizational account used to access Azure.
- **Subscription**: A container linked to your account. Resources within a subscription share the same billing relationship.
- **Billing**: Each subscription generates a separate bill.

### Types of Subscriptions:
- **Free Tier**: Includes $200 in credits and access to many free services for 12 months.
- **Pay-As-You-Go**: Charges you based on usage.
- **Enterprise Agreement**: Designed for large organizations with customized pricing.

---

## **2. Creating Resources**

Azure resources include virtual machines, databases, storage accounts, and more. Resources are grouped within **resource groups** for easy management.

### Steps to Create a Resource in the Azure Portal:
1. Log in to the [Azure Portal](https://portal.azure.com).
2. Click on **Create a Resource**.
3. Choose a resource type (e.g., Virtual Machine, Storage Account).
4. Provide configuration details like name, region, and pricing tier.
5. Assign the resource to a **Resource Group**.
6. Click **Review + Create** to validate the configuration, then click **Create**.

---

## **3. Searching Resources**

Searching resources is crucial for managing complex Azure environments.

### Using the Azure Portal:
1. Navigate to the **Search Bar** at the top of the portal.
2. Enter the resource name, type, or tags.
3. Select the resource from the search results to view or manage it.

### Using Azure CLI:
```bash
az resource list --name <resource-name>
```

### Using PowerShell:
```powershell
Get-AzResource -Name <resource-name>
```

---

## **4. Removing Resources**

Azure resources can be removed when no longer needed to avoid unnecessary costs.

### Using the Azure Portal:
1. Locate the resource in the portal.
2. Open the resource and click **Delete**.
3. Confirm the deletion.

### Using Azure CLI:
```bash
az resource delete --name <resource-name> --resource-group <resource-group-name>
```

### Using PowerShell:
```powershell
Remove-AzResource -Name <resource-name> -ResourceGroupName <resource-group-name>
```

---

## **5. Azure CLI and PowerShell**

Azure CLI and PowerShell are powerful tools for managing Azure resources programmatically.

### **Azure Cloud Shell**
Azure Cloud Shell is an interactive, browser-based shell available in the Azure Portal. It supports both Bash (for Azure CLI) and PowerShell.

- **To Access Cloud Shell**: 
  - Log in to the Azure Portal.
  - Click the **Cloud Shell** icon in the top navigation bar.
- **Pre-installed Tools**: Includes Azure CLI, PowerShell, Git, and more.

### **Example: Azure CLI**
#### Create a Resource Group:
```bash
az group create -l westus -n CLITest-rg
```
- `-l`: Specifies the location (e.g., `westus`).
- `-n`: Specifies the resource group name.

### **Example: PowerShell**
#### Create a Resource Group:
```powershell
New-AzResourceGroup -Name PSTest-rg -Location westus
```

---

## **6. What is a Resource Group?**

A **Resource Group** is a container that holds related Azure resources. It simplifies resource management by grouping resources with similar lifecycle, permissions, or dependencies.

### Example:
Suppose you're deploying a web application. You can create a resource group called **WebApp-RG** that includes:
- A Virtual Machine for the application server.
- A Storage Account for files and media.
- A SQL Database for data storage.

---

## **7. Resource Group vs Subscription**

| **Aspect**           | **Resource Group**                          | **Subscription**                               |
|-----------------------|---------------------------------------------|------------------------------------------------|
| **Definition**        | A logical container for related resources. | A container for billing and access policies.   |
| **Scope**             | Grouped resources (e.g., VMs, databases).  | Can include multiple resource groups.          |
| **Billing**           | Not directly tied to billing.              | Generates a bill for all resources within it.  |
| **Purpose**           | Organizational and lifecycle management.   | Budgeting, billing, and overall access control.|

### Relationship:
- A **subscription** contains one or more **resource groups**.
- A **resource group** cannot span multiple subscriptions.

---

## **8. Management Group**

An **Azure Management Group** provides a way to organize multiple subscriptions under a single hierarchy. This is useful for enterprises managing multiple subscriptions.

### Features:
- **Policy Application**: Apply Azure Policies and Role-Based Access Control (RBAC) across subscriptions.
- **Hierarchy**: Create a tree-like structure for subscriptions.
- **Cost Management**: View aggregated costs across subscriptions.

### Example:
- Parent Management Group: **Organization-MG**
  - Child 1: **IT-MG** (Subscription for IT projects).
  - Child 2: **Marketing-MG** (Subscription for marketing campaigns).

**Command to Create Management Group (CLI)**:
```bash
az account management-group create --name <management-group-name>
```

---

## **1. Storage Account**

An **Azure Storage Account** is a service that provides scalable and secure cloud storage for unstructured and structured data. It supports various types of storage services, such as blobs, files, queues, tables, and disks.

### Types of Storage in Azure:
1. **Blob Storage**: Optimized for unstructured data like images, videos, and backups.
2. **File Storage**: Provides managed file shares for use in the cloud or on-premises.
3. **Queue Storage**: Enables message storage for reliable communication between applications.
4. **Table Storage**: Offers NoSQL storage for structured data.
5. **Disk Storage**: Persistent storage for Azure Virtual Machines.

### Steps to Create a Storage Account:
1. Log in to the [Azure Portal](https://portal.azure.com).
2. Navigate to **Create a Resource** > **Storage** > **Storage Account**.
3. Specify the following:
   - **Resource Group**: Assign or create a resource group.
   - **Region**: Choose the region where the data will be stored.
   - **Performance Tier**: Standard (cost-efficient) or Premium (low-latency).
   - **Replication**: LRS, ZRS, GRS, or RA-GRS (explained below).
4. Click **Review + Create** and then **Create**.

### Storage Redundancy Options:
| **Replication**       | **Description**                                                                                 |
|------------------------|-------------------------------------------------------------------------------------------------|
| **LRS**               | Locally Redundant Storage: Copies data within a single datacenter.                              |
| **ZRS**               | Zone-Redundant Storage: Replicates data across multiple availability zones in a region.         |
| **GRS**               | Geo-Redundant Storage: Copies data to a secondary region for disaster recovery.                 |
| **RA-GRS**            | Read-Access Geo-Redundant Storage: Adds read access to the secondary copy in a different region.|

---

## **2. SLA (Service Level Agreement)**

An **SLA** is a formal contract between a service provider (Azure) and its customers that defines the expected level of service. Azure SLAs typically guarantee:
1. **Uptime**: The percentage of time a service is available.
2. **Performance**: Commitments to response times and throughput.
3. **Remedies**: Compensation (usually credits) for SLA breaches.

### Uptime SLA Table for Azure Services:
| **Service**                    | **Uptime Guarantee**  |
|--------------------------------|-----------------------|
| **Virtual Machines**           | 99.9% (Single VM)    |
| **Storage Account**            | 99.9% - 99.99%       |
| **SQL Database (Basic)**       | 99.99%               |
| **Azure Kubernetes Service**   | 99.95%               |

### Uptime Example:
- **99.9% uptime** allows for 8.76 hours of downtime per year.
- **99.99% uptime** allows for only 52.56 minutes of downtime per year.

### Calculating Downtime from SLA:
To calculate downtime:
1. **Downtime (per month)** = (1 - Uptime%) × Total Minutes in a Month.
2. Example:
   - For a 99.9% SLA: `(1 - 0.999) × (30 days × 24 hours × 60 minutes)` = 43.2 minutes of allowed downtime.

---

## **3. SLA Calculator**

Azure provides an **SLA Calculator** to estimate the cumulative SLA for multiple services in a solution. If your application relies on multiple services, the combined SLA is lower than the individual SLAs.

### Combined SLA Formula:
\[
\text{Combined SLA} = \text{SLA(Service A)} \times \text{SLA(Service B)} \times \dots
\]

### Example:
An application using two services:
1. Service A: 99.95%
2. Service B: 99.9%

Combined SLA:
\[
99.95\% \times 99.9\% = 99.85\%
\]

You can use the [Azure SLA Calculator](https://azure.microsoft.com/en-us/sla-calculator/) to simplify this process.

---

## **4. Cost in Azure**

Azure's pricing is flexible, pay-as-you-go, and depends on factors like resource type, usage, region, and redundancy level.

### Azure Pricing Models:
1. **Pay-As-You-Go**: Charges based on actual usage.
2. **Reserved Instances**: Pre-pay for resources for 1 or 3 years at discounted rates.
3. **Spot Pricing**: Discounts for unused compute capacity (suitable for interruptible workloads).
4. **Free Tier**: Access to free services and credits for 12 months.

### Cost Factors:
- **Resource Type**: VMs, storage, or databases.
- **Region**: Costs vary between regions.
- **Performance Tier**: Standard or premium performance.
- **Usage**: Amount of storage, compute hours, or data transfer.

### Example Pricing for a Storage Account:
| **Service**                    | **Price (Approx.)**              |
|--------------------------------|----------------------------------|
| **Blob Storage (Hot Tier)**    | $0.0184 per GB per month         |
| **Blob Storage (Cool Tier)**   | $0.01 per GB per month           |
| **RA-GRS Replication**         | $0.04 per GB per month           |
| **Operations**                 | $0.0004 per 1,000 operations     |

### Estimating Costs:
To estimate the cost of resources:
1. Use the [Azure Pricing Calculator](https://azure.microsoft.com/en-us/pricing/calculator/).
2. Select the services you need.
3. Configure region, redundancy, and expected usage to get a cost estimate.

---

Azure Compute

4 types of compute service

- Virtual Machines
- App Services
- AKS
- Azure Functions

Virtual Machine Architecture
- Code
- Binarys/Librarys
- Guest OS
- Hypervisor
- HOST OS

VM Density

Steps for creating the VM in India

Connect to VM

Availability of VM

Availability concepts in Azure
  - Fault Domain
  - Update Domain
  - Availability Set
  - Availability Zone
