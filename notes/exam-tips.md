# Exam Tips — CLF-C02

## Before the exam
- Book via **AWS Certification (aws.training/certification)** → Pearson VUE (test center or online proctored).
- Online proctoring: quiet room, clean desk, valid ID, webcam, stable internet, system test beforehand.
- If English is not your first language, you may be eligible for the **ESL +30 minutes accommodation** — request it **before** booking/scheduling (check current AWS policy).
- Sleep well. Don't cram new services the night before — review [06 glossary](06-glossary-service-index.md).

## During the exam
- **Never leave a question blank** — no penalty for guessing.
- ~80 seconds per question. **Flag** long ones and return.
- **Read the last sentence first** (what is being asked), then the scenario.
- Eliminate two obviously wrong answers, then choose.
- Multiple-response: the question tells you how many to select — pick exactly that many.
- Watch keywords: **most cost-effective**, **least operational overhead**, **highly available**, **fully managed**, **serverless**, **minimum effort**, **fastest**, **secure**.
- AWS answers are usually the **managed/serverless** option; "do it yourself on EC2" is usually a distractor (unless control is required).
- Questions are conceptual — **don't overthink**; pick the service that matches the stated use case.

## Keyword → answer

| If you read… | Think… |
|---|---|
| "least operational overhead", "managed" | RDS, Lambda, Fargate, DynamoDB |
| "audit / who did what / API calls" | CloudTrail |
| "resource configuration history / compliance rules" | Config |
| "monitor performance / alarms / metrics" | CloudWatch |
| "compliance report download" | Artifact |
| "DDoS" | Shield |
| "SQL injection / XSS / web exploits" | WAF |
| "threat detection / compromised" | GuardDuty |
| "vulnerability scan" | Inspector |
| "sensitive data / PII in S3" | Macie |
| "single pane of security findings" | Security Hub |
| "investigate root cause" | Detective |
| "encryption keys" | KMS (CloudHSM if dedicated hardware) |
| "SSL/TLS certificates" | ACM |
| "store/rotate DB passwords" | Secrets Manager |
| "workforce SSO" | IAM Identity Center |
| "app customers sign-up/sign-in" | Cognito |
| "cost alerts" | Budgets |
| "cost analysis / forecast" | Cost Explorer |
| "estimate before deploy" | Pricing Calculator |
| "line-item cost data in S3" | Cost and Usage Report |
| "interruptible, cheapest" | Spot |
| "steady, long-term, commit" | Reserved Instances / Savings Plans |
| "own per-socket licenses" | Dedicated Hosts |
| "guarantee capacity in an AZ" | Capacity Reservations |
| "hybrid, dedicated private connection" | Direct Connect |
| "quick encrypted tunnel" | VPN |
| "global low-latency content" | CloudFront |
| "static IPs, global routing" | Global Accelerator |
| "DNS" | Route 53 |
| "decouple" | SQS |
| "notify many subscribers" | SNS |
| "event bus / schedule" | EventBridge |
| "workflow orchestration" | Step Functions |
| "infrastructure as code" | CloudFormation |
| "serverless function" | Lambda |
| "containers, no servers" | Fargate |
| "upload code, AWS runs it" | Elastic Beanstalk |
| "cheap simple VPS" | Lightsail |
| "SQL on S3" | Athena |
| "real-time streaming" | Kinesis |
| "data warehouse" | Redshift |
| "NoSQL ms latency" | DynamoDB |
| "in-memory cache" | ElastiCache |
| "graph" | Neptune |
| "shared Linux files" | EFS |
| "block storage for EC2" | EBS |
| "archive cheapest" | S3 Glacier Deep Archive |
| "large offline data transfer" | Snow Family |
| "migrate DB" / "convert schema" | DMS / SCT |
| "chatbot" | Lex |
| "build/train ML models" | SageMaker AI |

## Traps to watch
1. **Elasticity vs scalability** (elasticity = automatic, both directions).
2. **Shared responsibility**: guest OS on EC2 = customer; RDS engine patching = AWS; data & IAM = always customer.
3. **SG = stateful, allow-only, instance**; **NACL = stateless, allow+deny, subnet**.
4. **CloudTrail (who) vs CloudWatch (performance) vs Config (configuration)**.
5. **Shield Standard = free & automatic**; Advanced = paid. **WAF = layer 7**.
6. **Data IN is free; data OUT is charged.**
7. **Region ≠ AZ ≠ edge location.** CloudFront uses edge locations.
8. **Root user**: MFA, no access keys, only for root-only tasks.
9. **Spot** can be interrupted.
10. **Savings Plans (flexible) vs Reserved Instances (specific).**
11. **Support plans (v1.3)**: Basic = no technical cases; **Business Support+** = 24/7, minimum for production; **Enterprise Support** = designated TAM; **Unified Operations** = mission-critical, < 5 min. Legacy names (Developer, Business, On-Ramp) may still appear.
12. **S3 One Zone-IA = single AZ** (data lost if the AZ is lost).
13. **Instance store is ephemeral**; **EBS is persistent**.
14. **Cost allocation tags must be activated.**

## Last-day checklist
- [ ] 6 Well-Architected pillars · 6 CAF perspectives · 7 Rs · 6 advantages of cloud
- [ ] Shared responsibility table (EC2 / RDS / Lambda / S3)
- [ ] IAM: user/group/role/policy, root tasks, MFA
- [ ] Security services map (GuardDuty/Inspector/Macie/Detective/Security Hub/Shield/WAF)
- [ ] CloudTrail vs CloudWatch vs Config
- [ ] Compute/storage/database/network "which service" table
- [ ] S3 classes (order hot → cold)
- [ ] Pricing options + data transfer rules + cost tools + support plans
