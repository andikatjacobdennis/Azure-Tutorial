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

## **Azure Compute Services Overview**

### 1. **Virtual Machines (VMs)**
   - **Definition**: Azure Virtual Machines provide an Infrastructure as a Service (IaaS) that allows users to deploy and manage their operating systems, applications, and software configurations.
   - **Key Features**: Full OS control, custom configurations, scaling options, and availability.

### 2. **App Services**
   - **Definition**: A Platform as a Service (PaaS) for hosting web applications, RESTful APIs, and mobile app backends without managing the underlying infrastructure.
   - **Key Features**: Auto-scaling, DevOps integration, CI/CD support.

### 3. **Azure Kubernetes Service (AKS)**
   - **Definition**: A managed Kubernetes service that simplifies deploying, scaling, and managing containerized applications.
   - **Key Features**: Automated updates, security, monitoring, and integrated CI/CD pipelines.

### 4. **Azure Functions**
   - **Definition**: A serverless compute service that lets users run small pieces of code without provisioning or managing servers.
   - **Key Features**: Event-driven execution, pay-per-use model, and integration with Azure services like Event Grid and Logic Apps.

---

## **Virtual Machine Architecture**

Azure Virtual Machines are built on a layered architecture:

1. **Code**: Applications or services hosted on the VM.
2. **Binaries/Libraries**: The runtime dependencies or frameworks required by the code.
3. **Guest OS**: The operating system installed on the virtual machine (e.g., Windows, Linux).
4. **Hypervisor**: Software that virtualizes the physical hardware, allowing multiple VMs to run on a single host.
5. **Host OS**: The operating system running on the physical server, managed by Azure.
6. **VM Density**: The number of virtual machines that can run on a single host machine.

---

## **Steps to Create a Virtual Machine in Azure (India Region)**

1. **Log in to Azure Portal**
   - Go to [Azure Portal](https://portal.azure.com) and sign in with your credentials.

2. **Navigate to Virtual Machines**
   - Search for **Virtual Machines** in the top search bar and click **Create** > **Azure Virtual Machine**.

3. **Configure Basic Settings**
   - **Subscription**: Select your Azure subscription.
   - **Resource Group**: Create a new one or use an existing group.
   - **Region**: Select **India** (Central India, South India, or West India).
   - **Image**: Choose an OS image (e.g., Windows Server 2022, Ubuntu 20.04).
   - **Size**: Pick a VM size based on your workload.

4. **Configure Administrator Account**
   - Username: Enter a username.
   - Authentication Type: Select Password or SSH Public Key.
   - Password: If applicable, set a secure password.

5. **Networking**
   - Create or select a Virtual Network (VNet).
   - Configure Public IP address and Network Security Groups (NSGs).

6. **Disks and Advanced Settings**
   - Choose disk type (Standard HDD, Premium SSD).
   - Configure additional options like monitoring, auto-shutdown, and tags.

7. **Review and Create**
   - Review all configurations, validate, and click **Create**.

---

## **Connecting to a Virtual Machine**

1. **Using RDP (Windows VM)**
   - Download the RDP file from the Azure Portal.
   - Open the file and connect using the administrator username and password.

2. **Using SSH (Linux VM)**
   - Open a terminal and run:
     ```bash
     ssh username@<Public-IP>
     ```
   - Use your SSH key or password for authentication.

---

## **Availability of Virtual Machines**

Azure provides several options to enhance the availability and reliability of your VMs:

### **Fault Domain**
   - A logical group of hardware that shares a common power source and network switch.
   - Spreading VMs across multiple fault domains reduces the risk of hardware failures affecting all VMs.

### **Update Domain**
   - A logical group of VMs that are updated together during planned maintenance.
   - Ensures that updates occur without downtime for all VMs in a deployment.

### **Availability Set**
   - Groups VMs to distribute them across multiple fault domains and update domains.
   - Designed to protect against hardware failures and planned maintenance.

### **Availability Zone**
   - Physically separate data centers within an Azure region.
   - VMs deployed across Availability Zones provide high availability and resilience to data center failures.

---

### **Part 1: Deploying a Virtual Machine with ARM Templates**

**Azure Resource Manager Template Overview**  
Azure Resource Manager (ARM) templates are JSON files that define Azure resources. They help automate deployments, ensure consistency, and support infrastructure as code.

---

#### **Step 1: Using an Azure ARM Template**
1. **Download the Template**  
   Start with a predefined ARM template for a VM:
   - Download the template file `template.json` and a parameters file `parameters.json`.

2. **Deploy Using Azure CLI**
   Upload and deploy the ARM template using the Azure CLI:
   ```bash
   az deployment group create --resource-group optimized-vm-rg --template-file template.json --parameters parameters.json
   ```
   Replace `optimized-vm-rg` with your Azure Resource Group.

   **Explanation**:
   - `--template-file`: Specifies the JSON file defining resources.
   - `--parameters`: Provides customization via parameters.

---

### **Part 2: Configuring a VM Scale Set**

**VM Scale Set Overview**  
Azure VM Scale Sets allow you to automatically scale the number of VM instances to meet demand, ensuring high availability and cost management.

#### **Step 1: Increasing and Decreasing Instances**
1. **Increase by 1 Instance**:
   Scale up the VM Scale Set:
   ```bash
   az vmss scale --resource-group optimized-vm-rg --name MyScaleSet --new-capacity <current_capacity+1>
   ```

2. **Decrease by 1 Instance**:
   Scale down the VM Scale Set:
   ```bash
   az vmss scale --resource-group optimized-vm-rg --name MyScaleSet --new-capacity <current_capacity-1>
   ```

#### **Step 2: Check Provider Status**
Check the status of Microsoft Insights:
```bash
az provider show --namespace microsoft.insights -o table
```

---

### **Part 3: Using Azure Instance Metadata Service**

The Azure Instance Metadata Service (IMDS) provides information about the VM environment and scheduled events. It's accessible within the VM through HTTP.

#### **Step 1: Retrieve Instance Metadata**
Access metadata using a curl command:
```bash
curl -H "Metadata:true" "http://169.254.169.254/metadata/instance?api-version=2021-12-13"
```

#### **Step 2: Fetch Scheduled Events**
Fetch events like maintenance or VM restart schedules:
```bash
curl -H "Metadata:true" "http://169.254.169.254/metadata/scheduledevents?api-version=2020-07-01"
```

---

### **Part 4: Setting Up the Catalog App**

**Deploying an ASP.NET Core 8 Website**

#### **Step 1: Publish Your ASP.NET Core 8 Website**
1. Use the `dotnet` CLI to publish:
   ```bash
   dotnet publish -c Release -o ./publish
   ```

2. Transfer the published files to the Azure VM via RDP or SCP.

#### **Step 2: Install and Configure IIS**
1. **Install IIS**:
   Use PowerShell to install IIS on the VM:
   ```powershell
   Install-WindowsFeature -name Web-Server -IncludeManagementTools
   ```

2. **Install .NET 8 Hosting Bundle**:
   Download and install the .NET 8 runtime hosting bundle from the official Microsoft website.

3. **Configure the IIS Site**:
   - Point the IIS site to the folder containing the published application.
   - Ensure the application pool is configured for `.NET CLR Version v4.0`.

#### **Step 3: Test the Deployment**
Access the app in a browser using the VM's public IP or domain.

---

## **Setting Up a Node.js Application**
We’ll use the following commands to set up a Node.js application from a GitHub repository.

1. **Install Git:**
   ```bash
   sudo apt install git
   ```

2. **Update System Packages:**
   ```bash
   sudo apt update
   ```

3. **Install Node.js:**
   ```bash
   sudo apt install nodejs
   ```

4. **Clone the GitHub Repository:**
   ```bash
   sudo git clone https://github.com/memilavi/weatherAPI.git
   ```

5. **Navigate to the Application Directory:**
   ```bash
   cd weatherAPI
   ```

6. **Install npm:**
   ```bash
   sudo apt install npm
   ```

7. **Run the Application:**
   ```bash
   npm start
   ```

At this point, your Node.js application should be running locally. 

---

## **Understanding IP Addresses**

- **Private IP Address:** 
  Used within a private network for communication between internal resources. Private IPs cannot be accessed from the internet.

- **Public IP Address:**
  Used for communication between resources over the internet. Resources with a public IP are accessible globally.

### **How to Open a Private IP Address to the Public Internet**

1. **Assign a Public IP:** In Azure, assign a public IP to your resource (e.g., a VM or load balancer).
2. **Create a Network Security Rule:** Ensure the network security group allows inbound traffic on the desired port (e.g., port 80 for HTTP).
3. **Use Azure Firewall:** To secure the public endpoint while allowing access.

---

## **App Services in Azure**
Azure **App Services** is a fully managed platform for hosting web applications, RESTful APIs, and mobile backends.

### **Features of App Services:**
- Handles auto-scaling, load balancing, and patch management.
- Integrates with CI/CD pipelines for continuous deployment.
- Supports multiple programming languages (Node.js, Python, .NET, Java).

### **App Service Tiers**
Azure App Services come in different pricing tiers, each designed for specific use cases:
1. **Free and Shared (F1/D1):** Basic, shared hosting for testing.
2. **Basic (B1, B2, B3):** Dedicated computing resources.
3. **Standard (S1, S2, S3):** Additional features like auto-scaling and staging slots.
4. **Premium (P1v2, P2v2):** Optimized for production workloads.
5. **Isolated (I1, I2):** High security and scalability for enterprise needs.

### **Auto Scaling App Services**
App Services automatically scale out (add instances) or scale up (increase resources) based on:
- Metrics like CPU and memory usage.
- Scheduled rules for predictable traffic spikes.

---

## **Setting Up and Deploying a Web App**

### **Configuring Outbound IP Address**
An **outbound IP address** is used for your application’s communication with external services. Azure assigns these automatically. You can configure a static outbound IP by integrating a NAT Gateway.

---

## **Deployment Slots**

**Deployment Slots** allow you to deploy and test a new version of your application without affecting the production environment.

### **Benefits of Deployment Slots:**
- Perform A/B testing by routing a percentage of traffic to different slots.
- Rollback seamlessly by swapping slots if an update fails.

### **Using Deployment Slots**
1. **Change Traffic Percentage:**
   - Adjust the percentage of traffic directed to a specific slot in the Azure Portal.

2. **Deploying via Azure in VS Code:**
   - Use the Azure App Service extension in VS Code to deploy to specific slots.
   - Connect VS Code to your Azure subscription and select the desired slot during deployment.

3. **Swap Slots:**
   - Swap the staging slot with production once the new version is verified.

---

## **Deployment Types**

### **Basic Deployment**
Deploy your application directly to the production environment. Suitable for small projects with minimal risk.

### **Rolling Deployment**
Deploy updates in small increments across instances to ensure no downtime.

### **Blue-Green Deployment**
Use two environments: one for the live application (blue) and one for the new version (green). After testing, switch traffic to the green environment.

---

## **Azure Kubernetes Service (AKS)**

**AKS** is Azure’s managed Kubernetes service for deploying, scaling, and managing containerized applications.

### **Key Features of AKS:**
1. **Simplified Kubernetes Management:**
   - Automates upgrades and patching of Kubernetes clusters.
2. **Integration with Azure Services:**
   - Native integration with Azure Monitor, Azure DevOps, and more.
3. **Auto Scaling:**
   - Automatically scales clusters based on demand.

### **Steps to Deploy on AKS:**
1. **Create an AKS Cluster:**
   - Use the Azure Portal or CLI to create a Kubernetes cluster.
   ```bash
   az aks create --resource-group <resource-group> --name <cluster-name> --node-count 3 --enable-addons monitoring --generate-ssh-keys
   ```

2. **Connect to the Cluster:**
   - Install `kubectl` and connect to your cluster.
   ```bash
   az aks get-credentials --resource-group <resource-group> --name <cluster-name>
   ```

3. **Deploy Applications:**
   - Use `kubectl` to deploy and manage your containers.
   ```bash
   kubectl apply -f <deployment-file>.yaml
   ```

4. **Monitor and Scale:**
   - Use Azure Monitor and auto-scaling configurations.

---

## **Introduction to Containers**
Containers have revolutionized the way applications are developed, deployed, and managed. Below, we explore the basics of containers and their advantages over traditional virtual machines (VMs).

### **Containers vs. Virtual Machines (VMs)**
| **Feature**       | **Containers**                          | **Virtual Machines**                 |
|--------------------|------------------------------------------|---------------------------------------|
| **Isolation**      | Lightweight process isolation           | Full OS-level isolation               |
| **Startup Time**   | Starts in seconds                       | Takes minutes                         |
| **Resource Usage** | Shares OS kernel; uses fewer resources  | Requires full OS; higher resource use |
| **Portability**    | Consistent across environments          | Limited portability                   |

### **Why Containers?**
- **Efficiency**: Containers are lightweight, starting quickly and using fewer resources.
- **Portability**: Applications bundled in containers run the same way in any environment, reducing "it works on my machine" issues.
- **Scalability**: Easy to scale horizontally, making containers ideal for microservices.

---

## **Introduction to Docker**

### **Docker Architecture**
Docker simplifies containerization by providing tools and a platform to build, ship, and run containers. Here's an overview of its components:

1. **Docker Client**: Used to interact with the Docker daemon (`docker build`, `docker run`).
2. **Docker Daemon (Engine)**: The core service managing containers, images, and networks.
3. **Containers**: Lightweight instances of images running in isolated environments.
4. **Images**: Immutable, pre-configured environments (OS, dependencies, application).
5. **Docker Registry**: A repository for storing and sharing container images. Examples include Docker Hub and Azure Container Registry.
6. **Dockerfile**: A text file containing instructions to build a Docker image.

### **Dockerfile**
A `Dockerfile` is essential for automating the creation of Docker images. Below is a simple example:

```dockerfile
# Use base image
FROM node:16

# Set working directory
WORKDIR /app

# Copy package files
COPY package*.json ./

# Install dependencies
RUN npm install

# Copy app source code
COPY . .

# Expose port
EXPOSE 3000

# Run the app
CMD ["npm", "start"]
```

Build an image using a `Dockerfile`:
```bash
docker build -t my-app:1.0 .
```

---

## **Introduction to Kubernetes (K8s)**
Kubernetes is a container orchestration platform that automates deployment, scaling, and management of containerized applications.

### **Key Features**
- **Scalability**: Automatically scale containers based on demand.
- **Self-Healing**: Restarts failed containers and replaces unresponsive nodes.
- **Load Balancing**: Distributes traffic across containers.
- **Declarative Management**: Desired states are defined in YAML files.

### **Basic Kubernetes Terminology**
- **Pod**: The smallest deployable unit in Kubernetes; often contains one container.
- **Node**: A worker machine in a Kubernetes cluster.
- **Cluster**: A set of nodes managed by a master node.
- **Deployment**: Manages pods and ensures desired states are maintained.

---

## **Building and Pushing Images with Azure**
### **Azure Container Registry (ACR)**
ACR is a private registry to store Docker images securely. Here's how to build and push an image:

```bash
az acr build --image cart:v1 --registry <REGISTRY NAME> --file Dockerfile .
```

### **Steps to Work with Containers in Azure**
1. **Install Docker in VS Code**
   - Install the Docker extension in Visual Studio Code.
   - Install Docker Desktop on your local machine.

2. **Build an Image**
   Use the Azure CLI to build a container image:
   ```bash
   az acr build --image <IMAGE_NAME> --registry <REGISTRY_NAME> --file Dockerfile .
   ```

3. **Push to Registry**
   Push the image to ACR or Docker Hub for sharing.

---

## **Working with AKS (Azure Kubernetes Service)**
AKS simplifies the deployment and management of Kubernetes clusters in Azure.

### **Setup AKS Cluster**
1. **Install Kubernetes CLI**:
   ```bash
   az aks install-cli
   ```
2. **Set PATH**: Ensure `kubectl` is available in your system path.

3. **Authenticate with Azure**:
   ```bash
   az login
   ```

4. **Get Cluster Credentials**:
   Connect to your AKS cluster:
   ```bash
   az aks get-credentials --resource-group <RESOURCE_GROUP> --name <CLUSTER_NAME>
   ```

5. **Verify Nodes**:
   Ensure your cluster nodes are ready:
   ```bash
   kubectl get nodes
   ```

6. **Deploy Applications**:
   Apply your Kubernetes deployment configuration:
   ```bash
   kubectl apply -f deployment.yaml
   ```

### **Example deployment.yaml**
```yaml
apiVersion: apps/v1
kind: Deployment
metadata:
  name: cart-app
  labels:
    app: cart
spec:
  replicas: 3
  selector:
    matchLabels:
      app: cart
  template:
    metadata:
      labels:
        app: cart
    spec:
      containers:
      - name: cart
        image: <ACR_NAME>.azurecr.io/cart:v1
        ports:
        - containerPort: 3000
---
apiVersion: v1
kind: Service
metadata:
  name: cart-service
spec:
  selector:
    app: cart
  ports:
  - protocol: TCP
    port: 80
    targetPort: 3000
  type: LoadBalancer
```

### **Monitor the Deployment**
Check the status of your deployment and services:
```bash
kubectl get pods
kubectl get services
```

## **Azure Functions**

Azure Functions is a **serverless compute service** that allows you to run small pieces of code without worrying about the underlying infrastructure. These functions can be triggered by various events and are highly scalable.

### **Triggers vs. Bindings**

- **Triggers**: Triggers define **how a function starts**. They are event sources that invoke the function. For example:
  - **HTTP Trigger**: Activates the function when an HTTP request is received.
  - **Timer Trigger**: Activates based on a defined schedule.
  - **Queue Trigger**: Reacts to messages added to a storage queue.
  
  Example of a trigger in `function.json` for an HTTP trigger:
  ```json
  {
      "type": "httpTrigger",
      "direction": "in",
      "authLevel": "function",
      "methods": ["get", "post"]
  }
  ```

- **Bindings**: Bindings simplify the interaction with other Azure services. They connect functions to data or services **without writing extensive boilerplate code**. Bindings can be **input** (reading from a data source) or **output** (writing to a data source).

  Example of a binding:
  ```json
  {
      "type": "queue",
      "direction": "out",
      "name": "myQueueItem",
      "queueName": "myqueue",
      "connection": "AzureWebJobsStorage"
  }
  ```

  **Key Difference**: 
  - Triggers start a function, whereas bindings connect the function to external resources.

---

### **Hosting Plans**

Azure Functions can run on three hosting plans:

1. **Consumption Plan**:
   - **Pay-per-execution model**.
   - Autoscaling happens automatically.
   - Best for sporadic workloads or unpredictable traffic.

2. **Premium Plan**:
   - Fixed pre-warmed instances for **faster cold starts**.
   - Can connect to virtual networks.
   - Best for applications requiring high performance and predictable latency.

3. **Dedicated (App Service) Plan**:
   - Runs on **App Service plans**, which means predictable costs.
   - Ideal for applications that are part of a broader app service setup.

---

## **Durable Functions**

Durable Functions extend Azure Functions to handle **stateful workflows**. They enable **long-running orchestrations** by managing state automatically. 

- **Orchestrator Functions**: Define the workflow logic.
- **Activity Functions**: Perform specific tasks or operations.
- **Client Functions**: Start or signal orchestrators.

Example use cases:
- Chaining tasks (e.g., process orders step by step).
- Fan-out/fan-in for parallel processing.
- Handling human interaction (e.g., waiting for user approval).

---

## **Running Functions Locally**

You can develop and debug Azure Functions locally using the **Azure Functions Core Tools**. 

1. **Install Azure Functions Core Tools**:
   Run:
   ```bash
   npm install -g azure-functions-core-tools@4
   ```

2. **Create a New Function App**:
   Use the Azure Functions CLI to create a new project:
   ```bash
   func init MyFunctionApp --worker-runtime node
   ```

3. **Add a Function**:
   ```bash
   func new
   ```

4. **Run the Function Locally**:
   ```bash
   func start
   ```

5. Use tools like **Postman** or a browser to test HTTP triggers.

---

## **Running Functions in Azure**

1. **Publish to Azure**:
   From the Azure CLI:
   ```bash
   func azure functionapp publish <YourAppName>
   ```

2. **Monitor and Debug**:
   Use **Application Insights** to monitor logs, performance metrics, and errors.

---

## **How to Choose a Compute Type**

Choosing the right compute type in Azure depends on the application's needs:
- **Serverless (Azure Functions)**: Ideal for event-driven, short-lived tasks (e.g., data processing).
- **Containerized Workloads**: Use if portability and container orchestration are critical.
- **Logic Apps**: Best for workflows integrating multiple services with minimal coding.

---

## **More Compute Options**

### **Logic Apps**

Logic Apps is a **workflow automation platform** for integrating apps, data, and services. It is designed for scenarios like:
- Connecting on-premise and cloud systems.
- Automating workflows (e.g., approvals, email alerts).
- Visual designer simplifies the process.

---

### **Azure Container Instances (ACI)**

Azure Container Instances allows you to run **Docker containers directly in Azure**, without managing infrastructure. Key features:
- Fast and cost-effective container orchestration.
- Suitable for isolated tasks or microservices.
- Supports Linux and Windows containers.

---

### **App Service Container**

This allows you to deploy **containerized applications** in Azure App Service. Key advantages:
- Combines the flexibility of containers with the power of App Services.
- Provides features like custom domains, SSL, and scaling.
- Great for web apps needing container environments.

---

# Networking in Azure Tutorial

## Introduction to Networking in Azure
Azure provides a robust networking foundation for managing cloud resources. Networking in Azure revolves around **Virtual Networks (VNets)**, which allow you to securely connect, manage, and scale your cloud resources such as Virtual Machines (VMs), databases, and more. This tutorial will guide you through the basics of VNets, CIDR Notation, and related concepts.

---

## **1. Virtual Networks (VNets)**

A **Virtual Network (VNet)** in Azure acts as a private network in the cloud. It is a fundamental building block for managing connectivity and resource communication.

### **Key Features:**
1. **Resource Communication:**
   - Resources within a VNet can communicate directly with each other by default.
   - VNets are isolated from each other by default but can be connected via **peering**.

2. **Private Network:**
   - VNets operate like private networks, similar to **Virtual Private Cloud (VPC)** in AWS.

3. **Scope:**
   - **Region-specific:** Each VNet is scoped to a single Azure region.
   - **Subscription-specific:** Each VNet is also scoped to a single Azure subscription.

4. **Segmentation:**
   - VNets can be divided into smaller **subnets** to organize and isolate resources.

5. **Security:**
   - VNets can be protected with **Network Security Groups (NSGs)** to control inbound and outbound traffic.

---

### **VNet Connectivity Options:**
- **VNet Peering:**
  - Allows two VNets to connect and communicate with low latency.
  - Works across regions, enabling global connectivity.
  
- **ExpressRoute and VPN Gateway:**
  - Connect VNets to on-premises networks securely.

---

## **2. CIDR Notation**

CIDR (Classless Inter-Domain Routing) is a way to define IP address ranges for your networks. VNets and subnets use CIDR notation to specify address spaces.

### **CIDR Syntax:**
```
<IP Address>/<Prefix Length>
```

The prefix length determines the number of bits used for the network part of the address. The remaining bits define the range of host addresses.

---

### **CIDR Notation Examples**

#### **Example 1:**
```
109.186.149.240/24
```
- **Details:**
  - Prefix length: 24 bits (8 bits for each of the first three groups).
  - Range: The last 8 bits (256 addresses) are available for hosts.
  - Address range: `109.186.149.0` to `109.186.149.255` (256 addresses).

---

#### **Example 2:**
```
109.186.149.240/16
```
- **Details:**
  - Prefix length: 16 bits (8 bits for the first two groups).
  - Range: The last 16 bits (65,536 addresses) are available for hosts.
  - Address range: `109.186.0.0` to `109.186.255.255` (65,536 addresses).

---

#### **Example 3:**
```
109.186.149.240/20
```
- **Details:**
  - Prefix length: 20 bits (8 + 8 + 4 bits for the first two and part of the third group).
  - Range: The last 12 bits (4,096 addresses) are available for hosts.
  - Address range: `109.186.144.0` to `109.186.159.255` (4,096 addresses).

---

### **How the Range is Calculated for /20**

1. The **third octet (`149`)** is partially used for the network.
   - `149` in binary: `1001 0101`.
   - The **first 4 bits** of the third octet (`1001`) are fixed for the network.
   - The **last 4 bits** of the third octet (`0101`) and the entire fourth octet contribute to the host range.

2. **Third Octet Range**:
   - The first 4 bits (`1001`) correspond to **144** in decimal (start of the range).
   - The last 4 bits can vary, allowing values up to `159`.

3. **Fourth Octet Range**:
   - All 8 bits are available for the host range, from `0` to `255`.

4. **Final Address Range**:
   - Start: `XXX.XXX.144.0` (binary `XXXX XXXX.XXXX XXXX.1001 0000.0000 0000`).
   - End: `XXX.XXXX.159.255` (binary `XXXX XXXX.XXXX XXXX.1001 1111.1111 1111`).
     -  Here 144 is (1001 0000) and 159 is (1001 1111)
---

### **CIDR Size Calculation Tip**
To calculate the size of the address range:
```
Size = 2^(32 - Prefix Length)
```

#### **Examples:**
1. `109.186.149.240/24`

   ```math
    Size =  2^{(32 - 24)} = 2^8 = 256  addresses.
   ```

2. `109.186.149.240/20`

   ```math
   Size =  2^{(32 - 20)} = 2^{12} = 4,096  addresses.
    ```
---

## **3. Subnetting in VNets**
VNets can be divided into smaller **subnets** to organize resources. Subnets use portions of the VNet’s address space (defined in CIDR notation).

### **Subnet Benefits:**
- **Resource Isolation:** Separate resources for better management.
- **Traffic Control:** Use NSGs to control traffic flow.
- **Scalability:** Efficiently allocate IP ranges for resource growth.

---

## **4. Security with Network Security Groups (NSGs)**
- **NSGs** are firewall rules attached to subnets or individual resources within a VNet.
- They control **inbound** and **outbound** traffic based on rules.
- Example rules:
  - Allow HTTP traffic on port 80.
  - Deny all traffic from specific IP ranges.

---

### **5. CIDR Calculator Tool**
For ease in calculating address ranges and sizes, use a CIDR calculator:
- [CIDR Subnet Calculator](https://mxtoolbox.com/subnetcalculator.aspx)

---

## **1. Subnet**
A **subnet** is a logical segment within a Virtual Network (VNet). Subnets help organize and segregate network traffic for improved performance and security.

- **Key Features of a Subnet:**
  - Shares a subset of a VNet's IP address range.
  - Allows isolation of resources for better control and governance.
  - Resources like Virtual Machines (VMs) and Azure services are placed in subnets for optimized communication.

---

## **2. Creating a Virtual Network**
Virtual Networks (VNets) are the foundation of Azure networking. Follow these steps to create a VNet:

1. **Navigate to the Azure Portal:**
   - Go to **Create a Resource** > **Networking** > **Virtual Network**.
2. **Define the VNet Settings:**
   - **Name**: Specify the name of the VNet.
   - **Address Space**: Define the CIDR range (e.g., 10.0.0.0/16).
   - **Region**: Choose the Azure region.
3. **Add Subnets:**
   - Specify the name and subnet address range (e.g., 10.0.1.0/24).
4. **Review and Create:**
   - Validate settings and click **Create**.

---

## **3. Working with VNets**
Once a VNet is created, you can:
- Add additional **subnets** for resource isolation.
- Attach resources like Virtual Machines to the VNet.
- Configure **Network Security Groups (NSGs)** for access control.
- Enable **Service Endpoints** for secure Azure service connections.

---

## **4. Network Security Groups (NSGs)**
**NSGs** are essential for managing inbound and outbound traffic to Azure resources.

- **Security Rules**:
  - **Inbound Rules**: Control traffic entering the subnet/resource.
  - **Outbound Rules**: Control traffic leaving the subnet/resource.
  - Define rules based on **source**, **destination**, **protocol**, and **port range**.
  - For example, to allow HTTP traffic, create a rule with:
    - Source: Any
    - Destination: Any
    - Protocol: TCP
    - Port Range: 80
    - Action: Allow

---

## **5. Network Peering**
**Network Peering** connects VNets within the same or different Azure regions for seamless communication.

### **Using Network Peering**
1. Navigate to one of the VNets in the Azure Portal.
2. Select **Peerings** and click **Add**.
3. Specify the target VNet and set the peering configuration.
4. Enable **Gateway Transit** if needed for cross-region communication.
5. Once configured, resources in the peered VNets can communicate privately.

---

## **6. Network Topology**
Understanding and monitoring your Azure network topology is crucial for managing resources and diagnosing issues.

### **Network Watcher**
Azure's **Network Watcher** provides tools for:
- Diagnosing connectivity issues.
- Capturing network traffic with **Packet Capture**.
- Viewing a **Topology Map** of your VNet.

---

## **7. Secure VM Access**
Securing access to Virtual Machines is critical for maintaining data integrity and preventing unauthorized access.

### **JIT Access**
- Use **Just-In-Time (JIT) Access** to minimize exposure by granting time-limited access to VMs.

### **VPN**
- Establish secure connectivity using a **Virtual Private Network (VPN)**.

### **Jump Box**
- Deploy a Jump Box (or Bastion Host) as a gateway for managing other VMs.

### **Bastion**
- Azure **Bastion** provides secure, browser-based RDP and SSH access without exposing VMs to the internet.

---

## **8. Service Endpoint**
A **Service Endpoint** allows Azure resources in a VNet to securely connect to Azure services like Storage and SQL over the Microsoft backbone network.

---

## **9. Private Link**
**Private Link** enables private access to Azure services via private IP addresses in your VNet.

### **Service Endpoint vs Private Link**
| Feature             | Service Endpoint           | Private Link               |
|---------------------|----------------------------|----------------------------|
| **Connectivity**    | Over the Azure backbone    | Via private IPs in the VNet |
| **Access Control**  | At the subnet level        | Granular resource-level control |
| **Use Case**        | Access Azure services      | Access specific instances of services |

---

## **10. Access Restrictions**
- Use access restrictions to allow/deny traffic to Azure resources.
- Define rules based on IP address ranges, VNets, or service tags.

---

## **11. App Service Environment (ASE)**
The **App Service Environment (ASE)** is a fully isolated environment for running Azure App Services.

- Provides high security and scalability.
- Ideal for hosting sensitive or high-load applications.

---

## **12. Load Balancer**
Azure **Load Balancers** distribute traffic across resources for high availability.

### **Load Balancer Types**
1. **Basic Load Balancer**:
   - Suitable for small-scale deployments.
2. **Standard Load Balancer**:
   - Provides higher scalability, advanced diagnostics, and zone redundancy.

---

## **1. Azure Application Gateway Overview**
### Features:
- **Layer 7 Routing**: Routes requests based on HTTP headers, URLs, hostnames, etc.
- **SSL Termination**: Handles SSL decryption, reducing load on backend servers.
- **Autoscaling**: Automatically adjusts based on traffic demands.
- **Health Monitoring**: Continuously checks the health of backend endpoints.
- **WAF Integration**: Protects applications from malicious traffic.
  
### Use Cases:
- Hosting multiple web applications behind a single gateway.
- Enhancing application security with WAF.
- Improving application performance using connection multiplexing.
- Centralized control for routing HTTP/HTTPS traffic.

---

## **2. Azure WAF (Web Application Firewall)**
### What is Azure WAF?
Azure WAF is a cloud-native security feature within Azure Application Gateway. It defends web applications against vulnerabilities by filtering and monitoring HTTP/HTTPS requests based on predefined or custom rules.

### Modes:
1. **Detection Mode**: Logs threats but does not block them.
2. **Prevention Mode**: Actively blocks suspicious requests.

### Core Features:
- **OWASP Rules**: Predefined rulesets from the Open Web Application Security Project (OWASP).
- **Custom Rules**: Define rules to block or allow specific traffic based on IP, geolocation, or patterns.
- **Logging**: Logs all activities for audit and troubleshooting.
- **Integration**: Seamlessly integrates with Azure Monitor for advanced analytics.

### Steps to Set Up WAF:
1. **Create an Application Gateway**:
   - Navigate to the Azure portal.
   - Create a resource > Select *Application Gateway*.
   - Configure the resource group, region, and other settings.

2. **Enable WAF**:
   - During Application Gateway creation, choose the **WAF Tier**.
   - Configure WAF settings (Detection or Prevention mode).

3. **Define Rules**:
   - Select default OWASP rules or add custom rules.
   - Test in Detection mode before switching to Prevention mode.

4. **Associate Backend Pools**:
   - Add backend web servers or apps as a pool.
   - Configure HTTP/HTTPS listeners and routing rules.

---

## **3. Understanding Ports**
### Well-Known Ports (0–1023)
Ports in this range are reserved for core protocols and services:
| **Service**                        | **Port** |
|------------------------------------|----------|
| FTP (File Transfer Protocol - Data Transfer) | 20       |
| FTP (Control/Command)              | 21       |
| SSH (Secure Shell)                 | 22       |
| Telnet                             | 23       |
| SMTP (Simple Mail Transfer Protocol) | 25     |
| DNS (Domain Name System)           | 53       |
| HTTP (HyperText Transfer Protocol) | 80       |
| POP3 (Post Office Protocol v3)     | 110      |
| IMAP (Internet Message Access Protocol) | 143   |
| HTTPS (HTTP Secure)                | 443      |
| SNMP (Simple Network Management Protocol) | 161   |

---

### Registered Ports (1024–49151)
These are semi-standard ports often associated with specific applications:
| **Service**                        | **Port** |
|------------------------------------|----------|
| MySQL Database                     | 3306     |
| PostgreSQL Database                | 5432     |
| RDP (Remote Desktop Protocol)      | 3389     |
| SIP (Session Initiation Protocol - Unencrypted) | 5060  |
| SIP (Session Initiation Protocol - Encrypted) | 5061   |
| LDAP (Lightweight Directory Access Protocol) | 389   |
| SMB (Server Message Block)         | 445      |

---

## **4. Best Practices**
1. **Enable WAF Prevention Mode**: Switch from Detection to Prevention mode after thorough testing to protect live traffic.
2. **Secure Backend Communication**: Use HTTPS for communication between Application Gateway and backend servers.
3. **Restrict Access**: Use Network Security Groups (NSGs) to limit access to the Application Gateway subnet.
4. **Enable Logging**: Utilize Azure Monitor and Log Analytics for traffic insights.
5. **Keep Rules Updated**: Regularly update WAF rules to protect against new vulnerabilities.

---

## **5. Example Scenario**
Suppose you're hosting a multi-tier web application on Azure:
- The frontend (HTTP/HTTPS) is routed through Application Gateway with WAF enabled.
- Backend services, such as a MySQL database, use port **3306**.
- Administrators access virtual machines via RDP on port **3389**.

By configuring WAF rules and using the port mappings, you ensure secure traffic routing and mitigate potential threats to your web application.

---


Data in Azure

Major Database Features

