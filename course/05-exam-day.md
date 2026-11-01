<img src="../assets/part-5.svg" width="100%" alt="Part 5. Exam day"/>

How to read questions, a key-word map to answer fast, the checklist for the last hour, and 30 questions to test yourself.

## 5.1 How to answer

> [!TIP]
> **Good to know.** Aim for **about 85%** on practice exams before booking: the real exam usually feels about 10 points harder. There is no reason to target 100%: pass and move on to the next certification.

1. Read the **last sentence first**: what exactly is asked (cheapest? most available? least effort?).
2. Read the scenario and underline the key words.
3. **Eliminate** the two answers that are clearly wrong, then choose between the remaining two.
4. For multiple response, select **exactly** the number requested.
5. When unsure, prefer the **managed or serverless** service: AWS likes answers where AWS does the work.
6. Never leave a blank: wrong answers cost nothing.
7. A strange, very hard question may be one of the 15 unscored ones: do your best and move on.
8. About 80 seconds per question: flag long ones and come back at the end.

## 5.2 Key word → answer

| If you read | Think |
|---|---|
| audit, who made the API call | CloudTrail |
| metrics, alarm, billing alarm | CloudWatch |
| configuration history, compliance rules | Config |
| compliance report (SOC, PCI, ISO) | Artifact |
| DDoS | Shield |
| SQL injection, cross-site scripting | WAF |
| threat detection, compromised | GuardDuty |
| vulnerabilities, CVE | Inspector |
| personal data in S3 | Macie |
| investigate root cause | Detective |
| single security dashboard | Security Hub |
| employees, single sign-on, many accounts | IAM Identity Center |
| sign-in for app customers | Cognito |
| rotate database passwords | Secrets Manager |
| encryption keys | KMS (dedicated hardware: CloudHSM) |
| HTTPS certificate | Certificate Manager |
| estimate before building | Pricing Calculator |
| alert on cost | Budgets |
| analyze and forecast cost | Cost Explorer |
| most detailed billing | Cost and Usage Report |
| cheapest, can be interrupted | Spot |
| steady 1 to 3 years, flexible | Savings Plans |
| per-core licenses | Dedicated Hosts |
| guarantee capacity in an AZ | Capacity Reservation |
| decouple | SQS |
| notify many subscribers | SNS |
| events, schedules | EventBridge |
| workflow | Step Functions |
| SQL on files in S3 | Athena |
| real-time streaming | Kinesis |
| ETL | Glue |
| data warehouse | Redshift |
| NoSQL, millisecond, any scale | DynamoDB |
| cache in memory | ElastiCache |
| MongoDB | DocumentDB |
| graph, relationships | Neptune |
| shared Linux files | EFS |
| Windows file share | FSx for Windows File Server |
| disk for an EC2 instance | EBS |
| cheapest archive | S3 Glacier Deep Archive |
| unknown access pattern | S3 Intelligent-Tiering |
| on-premises apps using cloud storage | Storage Gateway |
| content close to users | CloudFront |
| DNS, domain | Route 53 |
| connect many VPCs | Transit Gateway |
| private connection to a service | PrivateLink |
| dedicated private line | Direct Connect |
| encrypted tunnel over the internet | Site-to-Site VPN |
| infrastructure as code | CloudFormation |
| upload code, AWS runs it | Elastic Beanstalk |
| simple server, fixed monthly price | Lightsail |
| containers without servers | Fargate |
| Kubernetes | EKS |
| code triggered by events | Lambda |
| elasticity | Auto Scaling |
| chatbot | Lex |
| text to speech / speech to text | Polly / Transcribe |
| build your own ML model | SageMaker AI |
| generative AI assistant | Amazon Q |
| contact center | Connect |
| send emails | SES |
| virtual desktop | WorkSpaces |
| business case for migration | Migration Evaluator |
| move servers as they are | Application Migration Service (rehost) |
| migrate a database | DMS (+ SCT to convert the schema) |
| best-practice checks on the account | Trusted Advisor |
| limits of a service | Service Quotas |
| designated TAM | Enterprise Support or Unified Operations |
| report abuse | Trust & Safety |
| community answers | re:Post |

## 5.3 Last-hour checklist

- The 6 advantages of cloud, the 6 Well-Architected pillars, the 6 CAF perspectives and 4 benefits, the 7 Rs
- Shared responsibility for EC2, RDS, Lambda, S3; root-only tasks; least privilege
- CloudTrail vs CloudWatch vs Config; the security services; security group vs network ACL
- Region, AZ, edge location; 4 factors to choose a Region; DR strategies with RPO and RTO
- S3 classes in order; EBS vs EFS vs instance store; database per need
- EC2 buying options; data transfer rules; cost tools; the 4 Support plans and the old names

## 5.4 Test yourself

> [!NOTE]
> **Note.** Cover the answers in italics, answer each question aloud, then check. Every wrong answer points to a section to re-read.

1. A startup does not want to buy hardware and wants to pay monthly for what it uses. Which advantage? *Trade fixed expense for variable expense.*
2. Which pillar includes "automatically recover from failure"? *Reliability.*
3. A company wants to move servers to AWS as fast as possible without changing them. Strategy? *Rehost.*
4. Which CAF perspective covers training and culture? *People.*
5. On Amazon EC2, who patches the operating system? *The customer.* On Amazon RDS, who patches the database engine? *AWS.*
6. An EC2 instance must read files in S3. What is the secure way? *Attach an IAM role to the instance.*
7. Which service shows who deleted an S3 bucket yesterday? *CloudTrail.*
8. An auditor wants AWS's PCI DSS report. Where? *AWS Artifact.*
9. You must block one malicious IP address for a whole subnet. What? *A network ACL with a deny rule.*
10. The website suffers SQL injection attempts. Service? *AWS WAF.*
11. Which service finds personal data stored in S3? *Amazon Macie.*
12. Employees should sign in once to reach 15 AWS accounts. Service? *IAM Identity Center.*
13. Your application must stay up if one data center fails. Design? *Instances in several Availability Zones behind a load balancer.*
14. Which DR strategy keeps a small but complete copy running in another Region? *Warm standby.*
15. Traffic varies a lot during the day. Which service adds and removes instances automatically? *EC2 Auto Scaling.*
16. Run code when a file is uploaded, without managing servers? *AWS Lambda.*
17. Logs must be kept 7 years for compliance and are almost never read. Cheapest storage? *S3 Glacier Deep Archive.*
18. Several Linux instances need the same shared files. Service? *Amazon EFS.*
19. A game needs a NoSQL database with millisecond latency at any scale. Service? *Amazon DynamoDB.*
20. Managers want sales trends over five years from huge data. Service? *Amazon Redshift.*
21. Users in Asia complain that images load slowly from your European website. Service? *Amazon CloudFront.*
22. A batch job can be interrupted and must be as cheap as possible. Purchasing option? *Spot Instances.*
23. A database runs 24/7 for the next 3 years. Cheapest option? *Reserved Instances (or a Savings Plan).*
24. Finance wants an email when the monthly forecast exceeds the budget. Tool? *AWS Budgets.*
25. Which is the minimum Support plan recommended for production workloads? *Business Support+.*
26. Which Support plans include a designated Technical Account Manager? *Enterprise Support and Unified Operations.*
27. Where do developers ask questions to the community? *AWS re:Post.*
28. Is data transferred into AWS from the internet charged? *No.*
29. Which service gives best-practice recommendations on cost, security, performance, fault tolerance and limits? *AWS Trusted Advisor.*
30. A company wants a cost estimate of its new architecture before building it. Tool? *AWS Pricing Calculator.*

Then practise with the 70 questions of this guide, the official AWS Practice Question Set (free on Skill Builder) and a free practice exam. Book the exam when you score 85% or more.

---

<p align="center">[← Billing, Pricing, and Support](04-billing-pricing-and-support.md) &nbsp;·&nbsp; <a href="../README.md">Contents</a> &nbsp;·&nbsp; [Practice questions →](../practice/practice-questions.md)</p>
