# Azure data storage options

- Survey the data storage options in Azure
- Explore how Azure can meet your business demands for storing and analyzing data
- Compare Azure data options with on-premises storage

Context sales learning portal that you are looking to expand with content.

You're looking for a storage solution that is `secure`, `durable`, `scalable`, and easily `accessible` from across the globe.

Thinking about storing data in the cloud.

Concerns: `security`, `backup`, and `disaster recovery` and `manage` cloud-hosted data

- **Automated backup and recovery**: mitigates the risk of losing your data if there is any unforeseen failure or interruption.
- **Replication across the globe**: copies your data to protect it against any planned or unplanned events, such as scheduled maintenance or hardware failures. You can choose to replicate your data at multiple locations across the globe.
- **Support for data analytics**: supports performing analytics on your data consumption.
- **Encryption capabilities**: data is encrypted to make it highly secure; you also have tight control over who can access the data.
- **Multiple data types**: Azure can store almost any type of data you need. It can handle video files, text files, and even large binary files like virtual hard disks. It also has many options for your relational and NoSQL data.
- **Data storage in virtual disks**: Azure also has the capability of storing up to 8 TB of data in its virtual disks. This is a significant capability when you're storing heavy data such as videos and simulations.
- **Storage tiers**: storage tiers to prioritize access to data based on frequently used versus rarely used information.

## Types of data
- **Structured data.** Structured data is data that adheres to a schema, so all of the data has the same fields or properties. Structured data can be stored in a database table with `rows` and `columns`. Structured data relies on `keys` to indicate how one row in a table relates to data in another row of another table. Structured data is also referred to as `relational data`, as the data's schema defines the table of data, the fields in the table, and the clear relationship between the two. Structured data is straightforward in that it's `easy to enter, query, and analyze`. All of the data follows the same format. Examples of structured data include sensor data or financial data.

- **Semi-structured data**. Semi-structured data doesn't fit neatly into tables, rows, and columns. Instead, semi-structured data uses `tags` or `keys` that organize and provide a hierarchy for the data. Semi-structured data is also referred to as `non-relational or NoSQL data`.

- **Unstructured data**. Unstructured data encompasses data that has no designated structure to it. This also means that there are `no restrictions on the kinds of data it can hold`. For example, a blob can hold a PDF document, a JPG image, a JSON file, video content, etc. As such, unstructured data is becoming more prominent as businesses try to tap into new data sources.

## Different data storages
- **Azure SQL Database**, the engine of Sql Server. You can use the Azure Database Migration Service to migrate your Sql Server to the cloud. It uses the Microsoft Data Migration Assistant to generate reports to provide recommendations on things you should do before migrating. Thereafter it should be as simple as changing the Connection String in your apps.
- **Azure Cosmos DB**, globally distributed database service. Supports schema less data. Supports constantly changing data.
- **Azure Blob Storage**, unstructured, no restrictions on what type of data it can hold wether its PDFs, videos or anything else. Highly scalable. Can handle 1000s of simultaneous uploads. Has the ability to store up to 8 TB of data for virtual machines
- **Azure Data Lake Storage Gen2**, allows you to `perform analytics` on your data usage and `prepare reports`. Data Lake is a `large repository` that stores both `structured` and `unstructured data`. Combines the scalability and cost benefits of object storage with the reliability and performance of the Big Data file system capabilities
- **Azure files**, fully managed file shares in the cloud that are accessible via the industry standard `Server Message Block (SMB) protocol`. Applications running in Azure virtual machines or cloud services can mount a file storage share to access file data, just as a desktop application would mount a typical SMB share. Typical usage scenarios would be to share files anywhere in the world, diagnostic data, or application data sharing
- **Azure queue**, is a service for storing large numbers of messages that can be accessed from anywhere in the world. better durability across large workloads. components are decoupled, they can scale independently. Queue storage provides asynchronous message queueing for communication between application components, whether they are running in the cloud, on the desktop, on-premises, or on mobile devices. Typically, there are one or more `sender components` and one or more `receiver components`. Sender components `add messages to the queue`, while receiver components `retrieve messages from the front of the queue for processing`.
- **Disk storage**, Disk storage _provides disks for virtual machines_, _applications_, and _other services_ to access and use as they need, similar to how they would in on-premises scenarios. Disk storage allows data to be persistently stored and accessed from an attached virtual hard disk. The disks can be _managed_ or _unmanaged_ by Azure, and therefore managed and _configured by the user_.
Typical scenarios for using disk storage are: 
  - if you want to lift and shift applications that read and write data to persistent disks
  - if you are storing data that is not required to be accessed from outside the virtual machine to which the disk is attached.

  Types: from solid-state drives (SSDs) to traditional spinning hard disk drives (HDDs)
- **Storage Tiers**, three types:
  - Hot storage tier, optimized for storing data that is accessed frequently
  - Cool storage tier, optimized for data that is infrequently accessed and stored for at least 30 days
  - Archive storage tier, for data that is rarely accessed and stored for at least 180 days with flexible latency requirements
- **Encryption and replication**, Azure provides `security` and `high availability` to your data through encryption and replication features.

  Encryption for storage services:
  - **Azure Storage Service Encryption (SSE)** for data at rest helps you secure your data to meet the organization's security and regulatory compliance. It encrypts the data before storing it and decrypts the data before retrieving it. The encryption and decryption are transparent to the user.
  - **Client-side encryption** is where the data is already encrypted by the client libraries. Azure stores the data in the encrypted state at rest, which is then decrypted during retrieval.
  
  Replication for storage availability
A replication type is set up when you create a storage account. The replication feature ensures that your data is durable and always available. Azure provides regional and geographic replications to protect your data against natural disasters and other local disasters like fire or flooding.

## Comparison between Azure data storage and On Premise

- **Cost effectiveness**, An on-premises storage solution requires dedicated hardware that needs to be purchased, installed, configured, and maintained. This can be a significant up-front expense (or capital cost). Change in requirements can require investment in new hardware. Your hardware needs to be capable of handling peak demand which means it may sit idle or be under-utilized in off-peak times.

Azure data storage provides a pay-as-you-go pricing model which is often appealing to businesses as an operating expense instead of an upfront capital cost. It's also scalable, allowing you to scale up or scale out as demand dictates and scale back when demand is low. You are charged for data services only as you need them.
- **Reliability**, On-premises storage requires data backup, load balancing, and disaster recovery strategies. These can be challenging and expensive as they often each need dedicated servers requiring a significant investment in both hardware and IT resources.

Azure data storage provides data backup, load balancing, disaster recovery, and data replication as services to ensure data safety and high availability.
- **Storage types**, Sometimes multiple different storage types are required for a solution, such as file and database storage. An on-premises approach often requires numerous servers and administrative tools for each storage type.

Azure data storage provides a variety of different storage options including distributed access and tiered storage. This makes it possible to integrate a combination of storage technologies providing the best storage choice for each part of your solution.
- **Agility**, Requirements and technologies change. For an on-premises deployment this may mean provisioning and deploying new servers and infrastructure pieces, which is a time consuming and expensive activity.

Azure data storage gives you the flexibility to create new services in minutes. This flexibility allows you to change storage back-ends quickly without needing a significant hardware investment.

