# Week 9: Architecture Design Principles and Cost Optimization - Practice Questions

Based on the provided PDF, here are 30 recommended questions focusing on Cost Explorer, Budgets, Savings Plans, Trusted Advisor, and Well-Architected Framework concepts suitable for Week 9.

### Question 1 (PDF Q#24)
**Topic:** Cost Analysis (EC2)
**Question:**
A company observes an increase in Amazon EC2 costs in its most recent bill. The billing team notices unwanted vertical scaling of instance types for a couple of EC2 instances. A solutions architect needs to create a graph comparing the last 2 months of EC2 costs and perform an in-depth analysis to identify the root cause of the vertical scaling. How should the solutions architect generate the information with the LEAST operational overhead?
**Options:**
A. Use AWS Budgets to create a budget report and compare EC2 costs based on instance types.
B. Use Cost Explorer's granular filtering feature to perform an in-depth analysis of EC2 costs based on instance types.
C. Use graphs from the AWS Billing and Cost Management dashboard to compare EC2 costs based on instance types for the last 2 months.
D. Use AWS Cost and Usage Reports to create a report and send it to an Amazon S3 bucket. Use Amazon QuickSight with Amazon S3 as a source to generate an interactive graph based on instance types.

### Question 2 (PDF Q#50)
**Topic:** Patching / Operational Excellence
**Question:**
A company has a production workload that runs on 1,000 Amazon EC2 Linux instances. The workload is powered by third-party software. The company needs to patch the third-party software on all EC2 instances as quickly as possible to remediate a critical security vulnerability. What should a solutions architect do to meet these requirements?
**Options:**
A. Create an AWS Lambda function to apply the patch to all EC2 instances.
B. Configure AWS Systems Manager Patch Manager to apply the patch to all EC2 instances.
C. Schedule an AWS Systems Manager maintenance window to apply the patch to all EC2 instances.
D. Use AWS Systems Manager Run Command to run a custom command that applies the patch to all EC2 instances.

### Question 3 (PDF Q#140)
**Topic:** Cost Optimization (Compute)
**Question:**
A solutions architect needs to help a company optimize the cost of running an application on AWS. The application will use Amazon EC2 instances, AWS Fargate, and AWS Lambda for compute within the architecture. The EC2 instances will run the data ingestion layer of the application. EC2 usage will be sporadic and unpredictable. Workloads that run on EC2 instances can be interrupted at any time. The application front end will run on Fargate, and Lambda will serve the API layer. The front-end utilization and API layer utilization will be predictable over the course of the next year. Which combination of purchasing options will provide the MOST cost-effective solution for hosting this application? (Choose two.)
**Options:**
A. Use Spot Instances for the data ingestion layer
B. Use On-Demand Instances for the data ingestion layer
C. Purchase a 1-year Compute Savings Plan for the front end and API layer.
D. Purchase 1-year All Upfront Reserved instances for the data ingestion layer.
E. Purchase a 1-year EC2 instance Savings Plan for the front end and API layer.

### Question 4 (PDF Q#238)
**Topic:** Cost Monitoring (Budgets)
**Question:**
A company wants to experiment with individual AWS accounts for its engineer team. The company wants to be notified as soon as the Amazon EC2 instance usage for a given month exceeds a specific threshold for each account. What should a solutions architect do to meet this requirement MOST cost-effectively?
**Options:**
A. Use Cost Explorer to create a daily report of costs by service. Filter the report by EC2 instances. Configure Cost Explorer to send an Amazon Simple Email Service (Amazon SES) notification when a threshold is exceeded.
B. Use Cost Explorer to create a monthly report of costs by service. Filter the report by EC2 instances. Configure Cost Explorer to send an Amazon Simple Email Service (Amazon SES) notification when a threshold is exceeded.
C. Use AWS Budgets to create a cost budget for each account. Set the period to monthly. Set the scope to EC2 instances. Set an alert threshold for the budget. Configure an Amazon Simple Notification Service (Amazon SNS) topic to receive a notification when a threshold is exceeded.
D. Use AWS Cost and Usage Reports to create a report with hourly granularity. Integrate the report data with Amazon Athena. Use Amazon EventBridge to schedule an Athena query. Configure an Amazon Simple Notification Service (Amazon SNS) topic to receive a notification when a threshold is exceeded.

### Question 5 (PDF Q#284)
**Topic:** Cost Reporting
**Question:**
As part of budget planning, management wants a report of AWS billed items listed by user. The data will be used to create department budgets. A solutions architect needs to determine the most efficient way to obtain this report information. Which solution meets these requirements?
**Options:**
A. Run a query with Amazon Athena to generate the report.
B. Create a report in Cost Explorer and download the report.
C. Access the bill details from the billing dashboard and download the bill.
D. Modify a cost budget in AWS Budgets to alert with Amazon Simple Email Service (Amazon SES).

### Question 6 (PDF Q#290)
**Topic:** EC2 Pricing (Flexibility)
**Question:**
A company hosts a web application on multiple Amazon EC2 instances. The EC2 instances are in an Auto Scaling group that scales in response to user demand. The company wants to optimize cost savings without making a long-term commitment. Which EC2 instance purchasing option should a solutions architect recommend to meet these requirements?
**Options:**
A. Dedicated Instances only
B. On-Demand Instances only
C. A mix of On-Demand Instances and Spot Instances
D. A mix of On-Demand Instances and Reserved Instances

### Question 7 (PDF Q#308)
**Topic:** Trusted Advisor
**Question:**
A company has multiple AWS accounts that use consolidated billing. The company runs several active high performance Amazon RDS for Oracle On-Demand DB instances for 90 days. The company’s finance team has access to AWS Trusted Advisor in the consolidated billing account and all other AWS accounts. The finance team needs to use the appropriate AWS account to access the Trusted Advisor check recommendations for RDS. The finance team must review the appropriate Trusted Advisor check to reduce RDS costs. Which combination of steps should the finance team take to meet these requirements? (Choose two.)
**Options:**
A. Use the Trusted Advisor recommendations from the account where the RDS instances are running.
B. Use the Trusted Advisor recommendations from the consolidated billing account to see all RDS instance checks at the same time.
C. Review the Trusted Advisor check for Amazon RDS Reserved Instance Optimization.
D. Review the Trusted Advisor check for Amazon RDS Idle DB Instances.
E. Review the Trusted Advisor check for Amazon Redshift Reserved Node Optimization.

### Question 8 (PDF Q#347)
**Topic:** Savings Plans (Flexibility)
**Question:**
A company has an application that is running on Amazon EC2 instances. A solutions architect has standardized the company on a particular instance family and various instance sizes based on the current needs of the company. The company wants to maximize cost savings for the application over the next 3 years. The company needs to be able to change the instance family and sizes in the next 6 months based on application popularity and usage. Which solution will meet these requirements MOST cost-effectively?
**Options:**
A. Compute Savings Plan
B. EC2 Instance Savings Plan
C. Zonal Reserved Instances
D. Standard Reserved Instances

### Question 9 (PDF Q#413)
**Topic:** Operational Excellence / SES
**Question:**
An ecommerce company is experiencing an increase in user traffic. The company’s store is deployed on Amazon EC2 instances as a two-tier web application consisting of a web tier and a separate database tier. As traffic increases, the company notices that the architecture is causing significant delays in sending timely marketing and order confirmation email to users. The company wants to reduce the time it spends resolving complex email delivery issues and minimize operational overhead. What should a solutions architect do to meet these requirements?
**Options:**
A. Create a separate application tier using EC2 instances dedicated to email processing.
B. Configure the web instance to send email through Amazon Simple Email Service (Amazon SES).
C. Configure the web instance to send email through Amazon Simple Notification Service (Amazon SNS).
D. Create a separate application tier using EC2 instances dedicated to email processing. Place the instances in an Auto Scaling group.

### Question 10 (PDF Q#417)
**Topic:** Savings Plans
**Question:**
A company uses Amazon EC2 instances and AWS Lambda functions to run its application. The company has VPCs with public subnets and private subnets in its AWS account. The EC2 instances run in a private subnet in one of the VPCs. The Lambda functions need direct network access to the EC2 instances for the application to work. The application will run for at least 1 year. The company expects the number of Lambda functions that the application uses to increase during that time. The company wants to maximize its savings on all application resources and to keep network latency between the services low. Which solution will meet these requirements?
**Options:**
A. Purchase an EC2 Instance Savings Plan Optimize the Lambda functions’ duration and memory usage and the number of invocations. Connect the Lambda functions to the private subnet that contains the EC2 instances.
B. Purchase an EC2 Instance Savings Plan Optimize the Lambda functions' duration and memory usage, the number of invocations, and the amount of data that is transferred. Connect the Lambda functions to a public subnet in the same VPC where the EC2 instances run.
C. Purchase a Compute Savings Plan. Optimize the Lambda functions’ duration and memory usage, the number of invocations, and the amount of data that is transferred. Connect the Lambda functions to the private subnet that contains the EC2 instances.
D. Purchase a Compute Savings Plan. Optimize the Lambda functions’ duration and memory usage, the number of invocations, and the amount of data that is transferred. Keep the Lambda functions in the Lambda service VPC.

### Question 11 (PDF Q#434)
**Topic:** Disaster Recovery / CloudFormation
**Question:**
A company hosts its application in the AWS Cloud. The application runs on Amazon EC2 instances behind an Elastic Load Balancer in an Auto Scaling group and with an Amazon DynamoDB table. The company wants to ensure the application can be made available in anotherAWS Region with minimal downtime. What should a solutions architect do to meet these requirements with the LEAST amount of downtime?
**Options:**
A. Create an Auto Scaling group and a load balancer in the disaster recovery Region. Configure the DynamoDB table as a global table. Configure DNS failover to point to the new disaster recovery Region's load balancer.
B. Create an AWS CloudFormation template to create EC2 instances, load balancers, and DynamoDB tables to be launched when needed Configure DNS failover to point to the new disaster recovery Region's load balancer.
C. Create an AWS CloudFormation template to create EC2 instances and a load balancer to be launched when needed. Configure the DynamoDB table as a global table. Configure DNS failover to point to the new disaster recovery Region's load balancer.
D. Create an Auto Scaling group and load balancer in the disaster recovery Region. Configure the DynamoDB table as a global table. Create an Amazon CloudWatch alarm to trigger an AWS Lambda function that updates Amazon Route 53 pointing to the disaster recovery load balancer.

### Question 12 (PDF Q#449)
**Topic:** Database Migration / Cost
**Question:**
A company runs its application on an Oracle database. The company plans to quickly migrate to AWS because of limited resources for the database, backup administration, and data center maintenance. The application uses third-party database features that require privileged access. Which solution will help the company migrate the database to AWS MOST cost-effectively?
**Options:**
A. Migrate the database to Amazon RDS for Oracle. Replace third-party features with cloud services.
B. Migrate the database to Amazon RDS Custom for Oracle. Customize the database settings to support third-party features.
C. Migrate the database to an Amazon EC2 Amazon Machine Image (AMI) for Oracle. Customize the database settings to support third-party features.
D. Migrate the database to Amazon RDS for PostgreSQL by rewriting the application code to remove dependency on Oracle APEX.

### Question 13 (PDF Q#450)
**Topic:** Well-Architected Framework
**Question:**
A company has a three-tier web application that is in a single server. The company wants to migrate the application to the AWS Cloud. The company also wants the application to align with the AWS Well-Architected Framework and to be consistent with AWS recommended best practices for security, scalability, and resiliency. Which combination of solutions will meet these requirements? (Choose three.)
**Options:**
A. Create a VPC across two Availability Zones with the application's existing architecture. Host the application with existing architecture on an Amazon EC2 instance in a private subnet in each Availability Zone with EC2 Auto Scaling groups. Secure the EC2 instance with security groups and network access control lists (network ACLs).
B. Set up security groups and network access control lists (network ACLs) to control access to the database layer. Set up a single Amazon RDS database in a private subnet.
C. Create a VPC across two Availability Zones. Refactor the application to host the web tier, application tier, and database tier. Host each tier on its own private subnet with Auto Scaling groups for the web tier and application tier.
D. Use a single Amazon RDS database. Allow database access only from the application tier security group.
E. Use Elastic Load Balancers in front of the web tier. Control access by using security groups containing references to each layer's security groups.
F. Use an Amazon RDS database Multi-AZ cluster deployment in private subnets. Allow database access only from application tier security groups.

### Question 14 (PDF Q#454)
**Topic:** Systems Manager Inventory
**Question:**
A company has resources across multiple AWS Regions and accounts. A newly hired solutions architect discovers a previous employee did not provide details about the resources inventory. The solutions architect needs to build and map the relationship details of the various workloads across all accounts. Which solution will meet these requirements in the MOST operationally efficient way?
**Options:**
A. Use AWS Systems Manager Inventory to generate a map view from the detailed view report.
B. Use AWS Step Functions to collect workload details. Build architecture diagrams of the workloads manually.
C. Use Workload Discovery on AWS to generate architecture diagrams of the workloads.
D. Use AWS X-Ray to view the workload details. Build architecture diagrams with relationships.

### Question 15 (PDF Q#455)
**Topic:** Budgets / Notifications
**Question:**
A company uses AWS Organizations. The company wants to operate some of its AWS accounts with different budgets. The company wants to receive alerts and automatically prevent provisioning of additional resources on AWS accounts when the allocated budget threshold is met during a specific period. Which combination of solutions will meet these requirements? (Choose three.)
**Options:**
A. Use AWS Budgets to create a budget. Set the budget amount under the Cost and Usage Reports section of the required AWS accounts.
B. Use AWS Budgets to create a budget. Set the budget amount under the Billing dashboards of the required AWS accounts.
C. Create an IAM user for AWS Budgets to run budget actions with the required permissions.
D. Create an IAM role for AWS Budgets to run budget actions with the required permissions.
E. Add an alert to notify the company when each account meets its budget threshold. Add a budget action that selects the IAM identity created with the appropriate config rule to prevent provisioning of additional resources.
F. Add an alert to notify the company when each account meets its budget threshold. Add a budget action that selects the IAM identity created with the appropriate service control policy (SCP) to prevent provisioning of additional resources.

### Question 16 (PDF Q#459)
**Topic:** Cost Allocation Tags
**Question:**
A company uses AWS Organizations to run workloads within multiple AWS accounts. A tagging policy adds department tags to AWS resources when the company creates tags. An accounting team needs to determine spending on Amazon EC2 consumption. The accounting team must determine which departments are responsible for the costs regardless ofAWS account. The accounting team has access to AWS Cost Explorer for all AWS accounts within the organization and needs to access all reports from Cost Explorer. Which solution meets these requirements in the MOST operationally efficient way?
**Options:**
A. From the Organizations management account billing console, activate a user-defined cost allocation tag named department. Create one cost report in Cost Explorer grouping by tag name, and filter by EC2.
B. From the Organizations management account billing console, activate an AWS-defined cost allocation tag named department. Create one cost report in Cost Explorer grouping by tag name, and filter by EC2.
C. From the Organizations member account billing console, activate a user-defined cost allocation tag named department. Create one cost report in Cost Explorer grouping by the tag name, and filter by EC2.
D. From the Organizations member account billing console, activate an AWS-defined cost allocation tag named department. Create one cost report in Cost Explorer grouping by tag name, and filter by EC2.

### Question 17 (PDF Q#467)
**Topic:** Savings Plans Sharing
**Question:**
A company uses AWS Organizations. A member account has purchased a Compute Savings Plan. Because of changes in the workloads inside the member account, the account no longer receives the full benefit of the Compute Savings Plan commitment. The company uses less than 50% of its purchased compute power.
**Options:**
A. Turn on discount sharing from the Billing Preferences section of the account console in the member account that purchased the Compute Savings Plan.
B. Turn on discount sharing from the Billing Preferences section of the account console in the company's Organizations management account.
C. Migrate additional compute workloads from another AWS account to the account that has the Compute Savings Plan.
D. Sell the excess Savings Plan commitment in the Reserved Instance Marketplace.

### Question 18 (PDF Q#492)
**Topic:** Service Catalog
**Question:**
A company has multiple AWS accounts for development work. Some staff consistently use oversized Amazon EC2 instances, which causes the company to exceed the yearly budget for the development accounts. The company wants to centrally restrict the creation of AWS resources in these accounts. Which solution will meet these requirements with the LEAST development effort?
**Options:**
A. Develop AWS Systems Manager templates that use an approved EC2 creation process. Use the approved Systems Manager templates to provision EC2 instances.
B. Use AWS Organizations to organize the accounts into organizational units (OUs). Define and attach a service control policy (SCP) to control the usage of EC2 instance types.
C. Configure an Amazon EventBridge rule that invokes an AWS Lambda function when an EC2 instance is created. Stop disallowed EC2 instance types.
D. Set up AWS Service Catalog products for the staff to create the allowed EC2 instance types. Ensure that staff can deploy EC2 instances only by using the Service Catalog products.

### Question 19 (PDF Q#499)
**Topic:** Direct Connect Cost
**Question:**
A company needs to minimize the cost of its 1 Gbps AWS Direct Connect connection. The company's average connection utilization is less than 10%. A solutions architect must recommend a solution that will reduce the cost without compromising security. Which solution will meet these requirements?
**Options:**
A. Set up a new 1 Gbps Direct Connect connection. Share the connection with another AWS account.
B. Set up a new 200 Mbps Direct Connect connection in the AWS Management Console.
C. Contact an AWS Direct Connect Partner to order a 1 Gbps connection. Share the connection with another AWS account.
D. Contact an AWS Direct Connect Partner to order a 200 Mbps hosted connection for an existing AWS account.

### Question 20 (PDF Q#505)
**Topic:** EC2 Auto Scaling Cost
**Question:**
A company has Amazon EC2 instances that run nightly batch jobs to process data. The EC2 instances run in an Auto Scaling group that uses On Demand billing. If a job fails on one instance, another instance will reprocess the job. The batch jobs run between 12:00 AM and 06:00 AM local time every day. Which solution will provide EC2 instances to meet these requirements MOST cost-effectively?
**Options:**
A. Purchase a 1-year Savings Plan for Amazon EC2 that covers the instance family of the Auto Scaling group that the batch job uses.
B. Purchase a 1-year Reserved Instance for the specific instance type and operating system of the instances in the Auto Scaling group that the batch job uses.
C. Create a new launch template for the Auto Scaling group. Set the instances to Spot Instances. Set a policy to scale out based on CPU usage.
D. Create a new launch template for the Auto Scaling group. Increase the instance size. Set a policy to scale out based on CPU usage.

### Question 21 (PDF Q#511)
**Topic:** Aurora Cost (Dev/Test)
**Question:**
A company is developing software that uses a PostgreSQL database schema. The company needs to configure multiple development environments and databases for the company's developers. On average, each development environment is used for half of the 8-hour workday. Which solution will meet these requirements MOST cost-effectively?
**Options:**
A. Configure each development environment with its own Amazon Aurora PostgreSQL database
B. Configure each development environment with its own Amazon RDS for PostgreSQL Single-AZ DB instances
C. Configure each development environment with its own Amazon Aurora On-Demand PostgreSQL-Compatible database
D. Configure each development environment with its own Amazon S3 bucket by using Amazon S3 Object Select

### Question 22 (PDF Q#512)
**Topic:** Backup Strategy
**Question:**
A company uses AWS Organizations with resources tagged by account. The company also uses AWS Backup to back up its AWS infrastructure resources. The company needs to back up all AWS resources. Which solution will meet these requirements with the LEAST operational overhead?
**Options:**
A. Use AWS Config to identify all untagged resources. Tag the identified resources programmatically. Use tags in the backup plan.
B. Use AWS Config to identify all resources that are not running. Add those resources to the backup vault.
C. Require all AWS account owners to review their resources to identify the resources that need to be backed up.
D. Use Amazon Inspector to identify all noncompliant resources.

### Question 23 (PDF Q#525)
**Topic:** Cost Explorer API
**Question:**
A company wants to add its existing AWS usage cost to its operation cost dashboard. A solutions architect needs to recommend a solution that will give the company access to its usage cost programmatically. The company must be able to access cost data for the current year and forecast costs for the next 12 months. Which solution will meet these requirements with the LEAST operational overhead?
**Options:**
A. Access usage cost-related data by using the AWS Cost Explorer API with pagination.
B. Access usage cost-related data by using downloadable AWS Cost Explorer report .csv files.
C. Configure AWS Budgets actions to send usage cost data to the company through FTP.
D. Create AWS Budgets reports for usage cost data. Send the data to the company through SMTP.

### Question 24 (PDF Q#543)
**Topic:** Savings Plans (Sharing)
**Question:**
A company runs Amazon EC2 instances in multiple AWS accounts that are individually bled. The company recently purchased a Savings Pian. Because of changes in the company’s business requirements, the company has decommissioned a large number of EC2 instances. The company wants to use its Savings Plan discounts on its other AWS accounts. Which combination of steps will meet these requirements? (Choose two.)
**Options:**
A. From the AWS Account Management Console of the management account, turn on discount sharing from the billing preferences section.
B. From the AWS Account Management Console of the account that purchased the existing Savings Plan, turn on discount sharing from the billing preferences section. Include all accounts.
C. From the AWS Organizations management account, use AWS Resource Access Manager (AWS RAM) to share the Savings Plan with other accounts.
D. Create an organization in AWS Organizations in a new payer account. Invite the other AWS accounts to join the organization from the management account.
E. Create an organization in AWS Organizations in the existing AWS account with the existing EC2 instances and Savings Plan. Invite the other AWS accounts to join the organization from the management account.

### Question 25 (PDF Q#552)
**Topic:** Savings Plans vs Reserved Instances
**Question:**
A company needs to optimize the cost of its Amazon EC2 instances. The company also needs to change the type and family of its EC2 instances every 2-3 months. What should the company do to meet these requirements?
**Options:**
A. Purchase Partial Upfront Reserved Instances for a 3-year term.
B. Purchase a No Upfront Compute Savings Plan for a 1-year term.
C. Purchase All Upfront Reserved Instances for a 1-year term.
D. Purchase an All Upfront EC2 Instance Savings Plan for a 1-year term.

### Question 26 (PDF Q#554)
**Topic:** EC2 Instance Families
**Question:**
A company's SAP application has a backend SQL Server database in an on-premises environment. The company wants to migrate its on-premises application and database server to AWS. The company needs an instance type that meets the high demands of its SAP database. On-premises performance data shows that both the SAP application and the database have high memory utilization. Which solution will meet these requirements?
**Options:**
A. Use the compute optimized instance family for the application. Use the memory optimized instance family for the database.
B. Use the storage optimized instance family for both the application and the database.
C. Use the memory optimized instance family for both the application and the database.
D. Use the high performance computing (HPC) optimized instance family for the application. Use the memory optimized instance family for the database.

### Question 27 (PDF Q#559)
**Topic:** Cost Allocation Tags
**Question:**
A company hosts multiple applications on AWS for different product lines. The applications use different compute resources, including Amazon EC2 instances and Application Load Balancers. The applications run in different AWS accounts under the same organization in AWS Organizations across multiple AWS Regions. Teams for each product line have tagged each compute resource in the individual accounts. The company wants more details about the cost for each product line from the consolidated billing feature in Organizations. Which combination of steps will meet these requirements? (Choose two.)
**Options:**
A. Select a specific AWS generated tag in the AWS Billing console.
B. Select a specific user-defined tag in the AWS Billing console.
C. Select a specific user-defined tag in the AWS Resource Groups console.
D. Activate the selected tag from each AWS account.
E. Activate the selected tag from the Organizations management account.

### Question 28 (PDF Q#574)
**Topic:** Database Cost Optimization
**Question:**
A financial services company launched a new application that uses an Amazon RDS for MySQL database. The company uses the application to track stock market trends. The company needs to operate the application for only 2 hours at the end of each week. The company needs to optimize the cost of running the database. Which solution will meet these requirements MOST cost-effectively?
**Options:**
A. Migrate the existing RDS for MySQL database to an Aurora Serverless v2 MySQL database cluster.
B. Migrate the existing RDS for MySQL database to an Aurora MySQL database cluster.
C. Migrate the existing RDS for MySQL database to an Amazon EC2 instance that runs MySQL. Purchase an instance reservation for the EC2 instance.
D. Migrate the existing RDS for MySQL database to an Amazon Elastic Container Service (Amazon ECS) cluster that uses MySQL container images to run tasks.

### Question 29 (PDF Q#579)
**Topic:** Instance Scheduler
**Question:**
A company runs an application that uses Amazon RDS for PostgreSQL. The application receives traffic only on weekdays during business hours. The company wants to optimize costs and reduce operational overhead based on this usage. Which solution will meet these requirements?
**Options:**
A. Use the Instance Scheduler on AWS to configure start and stop schedules.
B. Turn off automatic backups. Create weekly manual snapshots of the database.
C. Create a custom AWS Lambda function to start and stop the database based on minimum CPU utilization.
D. Purchase All Upfront reserved DB instances.

### Question 30 (PDF Q#671)
**Topic:** Cost Anomaly Detection
**Question:**
A company runs its applications on Amazon EC2 instances. The company performs periodic financial assessments of its AWS costs. The company recently identified unusual spending. The company needs a solution to prevent unusual spending. The solution must monitor costs and notify responsible stakeholders in the event of unusual spending. Which solution will meet these requirements?
**Options:**
A. Use an AWS Budgets template to create a zero spend budget.
B. Create an AWS Cost Anomaly Detection monitor in the AWS Billing and Cost Management console.
C. Create AWS Pricing Calculator estimates for the current running workload pricing details.
D. Use Amazon CloudWatch to monitor costs and to identify unusual spending.
