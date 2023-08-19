# 3Tier-Web-Application-using-VPC-EC2--ALB-and-RDS:

**Project: Building a 3-Tier Application with AWS**

**Description:**
In this project, I designed and deployed a scalable 3-tier web application on Amazon Web Services (AWS) infrastructure. The architecture follows best practices for availability, scalability, and security, utilizing Virtual Private Cloud (VPC), EC2 instances, Application Load Balancer (ALB), and Amazon RDS (Relational Database Service).

**Architecture Overview:**

1. **Networking Layer (VPC):**
   - Created a Virtual Private Cloud (VPC) to isolate and manage the network resources.
   - Implemented public and private subnets for different tiers to enhance security and control data flow.

2. **Presentation Layer (Web Servers - Bastion Host):**
   - Deployed a bastion host EC2 instance in a public subnet to provide secure SSH access to the private instances.
   - Configured security groups to allow only specific IPs to access the bastion host.

3. **Application Layer (App Servers - AppServer 1 and 2):**
   - Launched two application server EC2 instances in private subnets.
   - Installed and configured application-specific software, frameworks, and dependencies.
   - Set up Auto Scaling for the app servers to ensure availability and handle varying loads.

4. **Load Balancing (ALB):**
   - Created an Application Load Balancer (ALB) in a public subnet to distribute incoming traffic across the application instances.
   - Configured health checks to ensure that only healthy instances receive traffic.

5. **Data Layer (RDS Database):**
   - Provisioned an Amazon RDS instance in a private subnet to host the application's relational database.
   - Chose an appropriate database engine (e.g., MySQL, PostgreSQL) and set up the necessary schemas and tables.






