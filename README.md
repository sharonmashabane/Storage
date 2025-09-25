# Storage

Storage in AWS Cloud Computing
>  What Storage Means in the Cloud

In cloud computing, storage refers to saving data, files, backups, or databases on remote servers managed by AWS instead of local hardware. Cloud storage is scalable, pay-as-you-go, highly available, and secure, making it suitable for everything from personal files to enterprise workloads.

> Types of AWS Storage
1. Object Storage – Amazon S3 (Simple Storage Service)

Stores data as objects (files + metadata).

Scales to store unlimited amounts of data.

Common use cases: backups, static websites, media hosting, data lakes.

Features: versioning, lifecycle rules, cross-region replication.

2. Block Storage – Amazon EBS (Elastic Block Store)

Attaches to EC2 instances like a hard drive.

Provides low-latency storage for running operating systems and applications.

Use cases: boot volumes, transactional databases, enterprise apps.

3. File Storage – Amazon EFS (Elastic File System)

Shared, managed file system that can be mounted by multiple EC2 instances.

Automatically scales as you add/remove files.

Use cases: shared storage for applications, content management, analytics.

4. Archival Storage – Amazon S3 Glacier & S3 Glacier Deep Archive

Low-cost storage for long-term archiving and compliance.

Data retrieval can take minutes to hours depending on cost tier.

Use cases: regulatory archives, medical records, historical data.

5. Hybrid & Edge Storage

AWS Storage Gateway → connects on-premises environments with AWS storage.

AWS Snow Family → physical devices for transferring large data volumes securely into AWS.

> Key Concepts Learned

Durability → AWS S3 provides 11 nines (99.999999999%) durability.

Availability → Data can be stored across multiple Availability Zones for fault tolerance.

Scalability → Automatically grows as storage needs increase.

Cost Optimization → Different storage classes (e.g., S3 Standard, S3 Infrequent Access, Glacier) help balance performance and price.

Security → Encryption at rest (KMS), encryption in transit (SSL/TLS), IAM policies for access control.

>  Hands-On Labs I Practiced

Created an S3 bucket and uploaded/downloaded objects.

Configured bucket policies and IAM roles for secure access.

Attached an EBS volume to an EC2 instance and formatted it.

Mounted an EFS file system to multiple EC2 instances simultaneously.

Set lifecycle rules to move data from S3 Standard to Glacier automatically.
