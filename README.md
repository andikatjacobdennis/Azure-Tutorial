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

Subscription and Account

Creating resourcea

Searching resource

removing resource

Azure CLI and powershell
  -  Azure cloud shell
  -  az group create -l westus -n CLITest-rg
  -  New-AzResourceGroup -Name PSTest-rg -Location westus 

What is a resource group with example



