# 06 · Glossary and A–Z Service Index

One-line definitions for every service/term likely on CLF-C02 (guide **v1.3**). Use for last-day review.

**Scope tags:** [v1.3] listed in v1.3 · [NEW] new/renamed in v1.3 · [LEGACY] (older guide / not listed now) · [OUT] explicitly out of scope. Untagged = general concept or supporting service.

## Concepts

| Term | Definition |
|---|---|
| **Region** | Geographic area with multiple AZs; independent |
| **Availability Zone (AZ)** | One or more data centers in a Region; isolated failure domain |
| **Edge location** | Point of presence for CloudFront/Route 53/Global Accelerator |
| **Elasticity** | Automatic scale out/in with demand |
| **Scalability** | Ability to handle growing load |
| **High availability** | Stays up if a component fails (multi-AZ) |
| **Fault tolerance** | Keeps running with no interruption on failure |
| **Durability** | Data is not lost (S3 = 11 nines) |
| **Agility** | Fast provisioning and experimentation |
| **CapEx / OpEx** | Upfront capital expense / ongoing operational expense |
| **TCO** | Total cost of ownership (all direct + indirect costs) |
| **IaC** | Infrastructure as Code (CloudFormation) |
| **Least privilege** | Grant only the minimum permissions needed |
| **Shared responsibility** | AWS secures **of** the cloud; customer secures **in** the cloud |
| **MFA** | Multi-factor authentication |
| **BYOL** | Bring your own license |
| **Rightsizing** | Match resource size to actual need |
| **Stateful / stateless** | Return traffic auto-allowed (SG) / must be explicitly allowed (NACL) |
| **Serverless** | You don't manage servers (Lambda, Fargate, DynamoDB, S3) |
| **Managed service** | AWS handles patching, backups, HA (RDS, DynamoDB) |
| **Well-Architected pillars** | Operational Excellence, Security, Reliability, Performance Efficiency, Cost Optimization, Sustainability |
| **CAF perspectives** | Business, People, Governance, Platform, Security, Operations |
| **7 Rs** | Retire, Retain, Rehost, Relocate, Repurchase, Replatform, Refactor |

## A–Z services

| Service | One-liner | Domain/Category |
|---|---|---|
| **Amazon API Gateway** | Create/publish/secure APIs | Networking / Integration |
| **AWS Activate** [OUT] | Startup credits & support | Customer engagement |
| **Amazon Aurora** | High-performance MySQL/PostgreSQL-compatible relational DB | Database |
| **AWS Amplify** | Build/host full-stack web & mobile apps | Frontend/mobile |
| **AWS AppConfig** [OUT] | Deploy app configuration / feature flags | Developer tools |
| **AWS AppSync** | Managed GraphQL API | Frontend/mobile |
| **Amazon AppStream 2.0** | Stream desktop apps to browsers | End-user computing |
| **Amazon Athena** | SQL queries on S3 (serverless) | Analytics |
| **AWS Artifact** | Compliance reports & agreements | Security |
| **AWS Audit Manager** | Continuously collect audit evidence | Security/Governance |
| **AWS Auto Scaling / EC2 Auto Scaling** | Automatic capacity adjustment | Compute/Management |
| **AWS Backup** | Centralized backup | Storage |
| **AWS Batch** | Batch computing at scale | Compute |
| **AWS Billing Conductor** [OUT] | Custom billing/pricing views | Cost mgmt |
| **AWS Budgets** | Cost/usage alerts | Cost mgmt |
| **AWS Certificate Manager (ACM)** | Manage SSL/TLS certificates | Security |
| **AWS Cloud9** | Cloud IDE | Developer tools |
| **AWS Cloud Adoption Framework (CAF)** | Cloud transformation guidance | Migration |
| **AWS CloudFormation** | IaC templates/stacks | Management |
| **Amazon CloudFront** | CDN | Networking |
| **AWS CloudHSM** | Dedicated hardware security module | Security |
| **AWS CloudShell** [OUT] | Browser-based CLI shell | Developer tools |
| **AWS CloudTrail** | API call audit log (who/what/when) | Management/Security |
| **Amazon CloudWatch** | Metrics, logs, alarms, dashboards | Management |
| **AWS CodeBuild** [v1.3] · **CodePipeline** [v1.3] · CodeArtifact [OUT] · CodeDeploy [OUT] · CodeCommit [LEGACY] · CodeStar [LEGACY] | Build / CI-CD pipeline / artifacts / deploy / Git repos / toolchain | Developer tools |
| **Amazon Cognito** | Sign-up/sign-in for app customers | Security |
| **Amazon Comprehend** | NLP: sentiment, entities | AI/ML |
| **AWS Compute Optimizer** | ML rightsizing recommendations | Management |
| **AWS Config** | Resource config history + compliance rules | Management |
| **Amazon Connect** | Cloud contact center | Business apps |
| **AWS Control Tower** | Multi-account landing zone governance | Management |
| **AWS Cost and Usage Report (CUR)** | Most detailed cost data in S3 | Cost mgmt |
| **AWS Cost Explorer** | Analyze/forecast costs | Cost mgmt |
| **AWS Data Exchange** [OUT] | Third-party datasets | Analytics |
| **AWS DataSync** | Online data transfer to AWS storage | Migration |
| **AWS Database Migration Service (DMS)** | Migrate databases with minimal downtime | Migration/DB |
| **Amazon Detective** | Investigate security findings | Security |
| **AWS Direct Connect** | Dedicated private connection to AWS | Networking |
| **AWS Directory Service** | Managed Microsoft Active Directory | Security |
| **Amazon DynamoDB** | Serverless NoSQL key-value DB | Database |
| **Amazon EBS** | Block storage for EC2 | Storage |
| **Amazon EC2** | Virtual servers | Compute |
| **Amazon ECR** | Container image registry | Containers |
| **Amazon ECS** | AWS container orchestration | Containers |
| **Amazon EFS** | Shared elastic file system (Linux/NFS) | Storage |
| **AWS Elastic Beanstalk** | Deploy apps; AWS manages infra | Compute |
| **AWS Elastic Disaster Recovery** | Recover servers after disaster | Storage/DR |
| **Elastic Load Balancing (ELB)** | Distribute traffic (ALB/NLB/GWLB) | Compute/Networking |
| **Amazon ElastiCache** | In-memory cache (Redis/Memcached) | Database |
| **Amazon EKS** | Managed Kubernetes | Containers |
| **Amazon EMR** | Managed Hadoop/Spark | Analytics |
| **Amazon EventBridge** | Serverless event bus | Integration |
| **AWS Fargate** | Serverless compute for containers | Serverless |
| **AWS Firewall Manager** | Central firewall rule management across accounts | Security |
| **Amazon FSx** | Managed Windows/Lustre/NetApp/OpenZFS file systems | Storage |
| **AWS Global Accelerator** | Static anycast IPs over AWS backbone | Networking |
| **AWS Glue** | Serverless ETL + Data Catalog | Analytics |
| **Amazon GuardDuty** | Intelligent threat detection | Security |
| **AWS Health Dashboard** | Service & account health events | Management/Support |
| **AWS IAM** | Users, groups, roles, policies | Security |
| **AWS IAM Identity Center** | Workforce SSO | Security |
| **Amazon Inspector** | Automated vulnerability scanning | Security |
| **AWS IoT Core** [v1.3] · Greengrass [OUT] | Connect devices / local edge IoT | IoT |
| **AWS IQ** [OUT] | Hire AWS-certified experts | Customer engagement |
| **Amazon Kendra** | ML enterprise search | AI/ML |
| **AWS KMS** | Managed encryption keys | Security |
| **Amazon Kinesis** | Real-time streaming data | Analytics |
| **AWS Lambda** | Serverless functions | Compute |
| **Amazon Lex** | Chatbots (conversational) | AI/ML |
| **AWS License Manager** | Track software licenses | Management |
| **Amazon Lightsail** | Simple VPS with predictable pricing | Compute |
| **AWS Local Zones** | Compute near population centers | Global infra |
| **Amazon Macie** | Discover sensitive data in S3 | Security |
| **AWS Managed Services (AMS)** [OUT] | AWS operates your infra | Customer engagement |
| **AWS Marketplace** | Buy third-party software | Cost/Partners |
| **Amazon MemoryDB** [OUT] | Durable in-memory Redis-compatible DB | Database |
| **AWS Migration Hub** | Track migrations | Migration |
| **Amazon MSK** [OUT] | Managed Kafka | Analytics |
| **Amazon Neptune** | Graph database | Database |
| **AWS Network Firewall** [OUT] | Managed VPC firewall | Security |
| **AWS Organizations** | Multi-account mgmt + consolidated billing + SCPs | Management |
| **AWS Outposts** | AWS infra in your data center | Compute/Hybrid |
| **Amazon OpenSearch Service** | Search & log analytics | Analytics |
| **Amazon Polly** | Text-to-speech | AI/ML |
| **AWS Pricing Calculator** | Estimate costs | Cost mgmt |
| **Amazon Quick** [NEW] (formerly QuickSight) | BI dashboards | Analytics [v1.3] |
| **AWS RAM** | Share resources across accounts | Security |
| **Amazon RDS** | Managed relational DB | Database |
| **Amazon Redshift** | Data warehouse | Database/Analytics |
| **Amazon Rekognition** | Image/video analysis | AI/ML |
| **Amazon Route 53** | DNS + health checks | Networking |
| **Amazon S3 / S3 Glacier** | Object storage / archive classes | Storage |
| **Amazon SageMaker AI** [NEW] (formerly SageMaker) | Build/train/deploy ML models | AI/ML [v1.3] |
| **AWS Schema Conversion Tool (SCT)** | Convert DB schema | Migration |
| **AWS Secrets Manager** | Store/rotate secrets | Security |
| **AWS Security Hub** | Aggregate security findings | Security |
| **AWS Service Catalog** | Approved product catalog | Management |
| **Amazon SES** | Bulk/transactional email | Business apps |
| **AWS Shield** | DDoS protection (Standard free / Advanced paid) | Security |
| **AWS Snow Family** | Physical devices for data transfer/edge | Migration |
| **Amazon SNS** | Pub/sub notifications | Integration |
| **Amazon SQS** | Message queue | Integration |
| **AWS Step Functions** | Workflow orchestration | Integration |
| **AWS Storage Gateway** | Hybrid cloud storage | Storage |
| **AWS Systems Manager** | Operate/patch/manage fleets | Management |
| **Amazon Textract** | Extract text/forms from documents | AI/ML |
| **Amazon Transcribe** | Speech-to-text | AI/ML |
| **AWS Transfer Family** [OUT] | SFTP/FTPS into S3/EFS | Migration |
| **Amazon Translate** | Language translation | AI/ML |
| **AWS Trusted Advisor** | Best-practice checks | Management/Support |
| **Amazon VPC** | Isolated virtual network | Networking |
| **AWS VPN** | Encrypted tunnel to AWS | Networking |
| **AWS WAF** | Web application firewall (L7) | Security |
| **AWS Wavelength** [OUT] | AWS at 5G network edge | Global infra |
| **AWS Well-Architected Tool** | Review workloads vs pillars | Management |
| **Amazon WorkSpaces** [v1.3] · **WorkSpaces Secure Browser** [NEW] (formerly WorkSpaces Web) | Virtual desktops / secure browser access | End-user computing |
| **AWS X-Ray** | Distributed tracing | Developer tools |
| **Amazon DocumentDB** [v1.3] | MongoDB-compatible document database | Database |
| **Amazon Q** [v1.3] | Generative-AI assistant | AI/ML |
| **AWS PrivateLink** [NEW] | Private connectivity to services (no public internet) | Networking |
| **AWS Transit Gateway** [NEW] | Hub connecting many VPCs and on-prem networks | Networking |
| **AWS Site-to-Site VPN / Client VPN** [NEW] | VPN for sites / individual users | Networking |
| **AWS Service Quotas** [NEW] | View/manage service limits | Management |
| **AWS Migration Evaluator** [NEW] | Build migration business case / TCO | Migration |
| **AWS Business Support+** [NEW] | Minimum recommended plan for production; 24/7; < 1 h prod down; < 30 min critical | Support |
| **AWS Enterprise Support** [NEW] | Designated TAM; < 15 min critical; Security Incident Response included | Support |
| **AWS Unified Operations** [NEW] | Mission-critical; < 5 min critical; continuous resiliency reviews | Support |
