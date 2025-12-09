# [AWS Well‑Architected Framework](https://docs.aws.amazon.com/pdfs/wellarchitected/latest/framework/wellarchitected-framework.pdf#welcome)
The Well‑Architected Framework is a set of best practices and guidelines for developers, architects and teams to design and operate workloads on AWS in an optimal way. This Framework contains six pillars.

# The Six Pillars (Core of the Framework)
These pillars reflect best practices for creating well-architected cloud applications
## 1. Operational Excellence
- Operational excellence (OE) is a commitment to build software correctly while consistently delivering a great customer experience. The operational excellence pillar contains best practices for organizing your team, designing your workload, operating it at scale, and evolving it over time.
- **Goal:** Automate, monitor, and improve operations.
- **Developer Actions:**
  - Use Infrastructure as Code (CloudFormation, CDK).
  - Implement CI/CD pipelines (CodePipeline, CodeBuild, CodeDeploy).
  - Add logging & tracing (CloudWatch Logs, X-Ray).
- **Key Services:** CloudFormation, CDK, CodePipeline, CloudWatch, X-Ray.

## 2. Security
- The Security pillar encompasses the ability to protect data, systems, and assets to take advantage of cloud technologies to improve your security.
- **Goal:** Protect data and systems.
- **Developer Actions:**
  - Apply least privilege (IAM roles, policies).
  - Encrypt data (KMS, SSE for S3).
  - Avoid hardcoded credentials; use environment variables or Secrets Manager.
- **Key Services:** IAM, KMS, Secrets Manager, CloudTrail.

## 3. Reliability
- The Reliability pillar encompasses the ability of a workload to perform its intended functioncorrectly and consistently when it’s expected to. This includes the ability to operate and testthe workload through its total lifecycle.
- **Goal:** Ensure workload recovers from failures.
- **Developer Actions:**
  - Design fault-tolerant apps (Multi-AZ, Auto Scaling).
  - Implement retry logic & exponential backoff in code.
  - Use health checks and graceful degradation.
- **Key Services:** Auto Scaling, ALB, Route 53, S3 versioning.

## 4. Performance Efficiency
- The performance efficiency pillar includes the ability to use cloud resources efficiently to meetperformance requirements, and to maintain that efficiency as demand changes and technologiesevolve.
- **Goal:** Use resources efficiently.
- **Developer Actions:**
  - Choose right compute (Lambda for serverless, EC2 for flexibility).
  - Use caching (CloudFront, ElastiCache).
  - Optimize DB queries (DynamoDB, RDS).
- **Key Services:** Lambda, API Gateway, DynamoDB, CloudFront.

## 5. Cost Optimization
- The Cost Optimization pillar includes the ability to run systems to deliver business value at thelowest price point.
- **Goal:** Reduce unnecessary costs.
- **Developer Actions:**
  - Use serverless where possible.
  - Enable S3 lifecycle policies for storage.
  - Monitor costs with AWS Cost Explorer.
- **Key Services:** Lambda, S3 lifecycle, Cost Explorer.

## 6. Sustainability
- The Sustainability pillar focuses on environmental impacts, especially energy consumptionand efficiency, since they are important levers for architects to inform direct action to reduceresource usage.
- **Goal:** Minimize environmental impact.
- **Developer Actions:**
  - Optimize resource usage.
  - Use managed services to reduce overhead.
- **Key Services:** Serverless (Lambda), Auto Scaling.
