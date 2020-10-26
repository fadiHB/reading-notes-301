# What is SQL?

SQL Server is a relational database management system, or RDBMS, developed and marketed by Microsoft.

Similar to other RDBMS software, SQL Server is built on top of SQL, a standard programming language for interacting with the relational databases. SQL server is tied to Transact-SQL, or T-SQL, the Microsoft’s implementation of SQL that adds a set of proprietary programming constructs.

SQL Server works exclusively on Windows environment for more than 20 years. In 2016, Microsoft made it available on Linux. SQL Server 2017 became generally available in October 2016 that ran on both Windows and Linux

## SQL Server Architecture

The following diagram illustrates the architecture of the SQL Server

![GitHub Logo](img07/What-is-SQL-Server-SQL-Server-Architecture.png)

SQL Server consists of two main components:

1. Database Engine
2. SQLOS

### Database Engine
The core component of the SQL Server is the Database Engine. The Database Engine consists of a relational engine that processes queries and a storage engine that manages database files, pages, pages, index, etc. The database objects such as stored procedures, views, and triggers are also created and executed by the Database Engine.

### Relational Engine
The Relational Engine contains the components that determine the best way to execute a query. The relational engine is also known as the query processor.

The relational engine requests data from the storage engine based on the input query and processed the results.

Some tasks of the relational engine include querying processing, memory management, thread and task management, buffer management, and distributed query processing.

### Storage Engine
The storage engine is in charge of storage and retrieval of data from the storage systems such as disks and SAN.

### SQLOS
Under the relational engine and storage engine is the SQL Server Operating System or SQLOS.

SQLOS provides many operating system services such as memory and I/O management. Other services include exception handling and synchronization services.

### SQL Server Services and Tools
Microsoft provides both data management and business intelligence (BI) tools and services together with SQL Server.

For data management, SQL Server includes SQL Server Integration Services (SSIS), SQL Server Data Quality Services, and SQL Server Master Data Services. To develop databases, SQL Server provides SQL Server Data tools; and to manage, deploy, and monitor databases SQL Server has SQL Server Management Studio (SSMS).

For data analysis, SQL Server offers SQL Server Analysis Services (SSAS). SQL Server Reporting Services (SSRS) provides reports and visualization of data. The Machine Learning Services technology appeared first in SQL Server 2016 which was renamed from the R Services.

### SQL Server Editions
SQL Server has four primary editions that have different bundled services and tools. Two editions are available free of charge:

SQL Server Developer edition for use in database development and testing.

SQL Server Expression for small databases with the size up to 10 GB of disk storage capacity.

For larger and more critical applications, SQL Server offers the Enterprise edition that includes all SQL server’s features.

SQL Server Standard Edition has partial feature sets of the Enterprise Edition and limits on the Server regarding the numbers of processor core and memory that can be configured.