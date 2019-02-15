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


