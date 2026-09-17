# AWS-SCS-C02-Security-Specialty-Study-Guide-Exam-Notes
Community study guide for the retired AWS SCS-C02 Security Specialty exam, covering AWS security architecture, identity, data protection, monitoring, incident response, and exam preparation.
# AWS SCS-C02 Security Specialty Study Guide

> Community study guide for AWS Certified Security - Specialty (SCS-C02).

> **Important:** SCS-C02 was the previous version of the AWS Certified Security - Specialty exam and was in use until **December 1, 2025**. The current exam version is **SCS-C03**. This repository is specifically for historical SCS-C02 preparation and reference. Verify the current exam version with AWS before registering.

## Introduction

This repository provides concise SCS-C02 study notes, AWS security concepts, practical lab ideas, revision guidance, and legitimate exam-preparation resources.

The material is designed for security professionals, cloud engineers, architects, administrators, and AWS practitioners who needed to understand how to secure AWS workloads and applications.

## Exam Overview

| Item | SCS-C02 Details |
|---|---|
| Vendor | Amazon Web Services (AWS) |
| Certification | AWS Certified Security - Specialty |
| Exam code | SCS-C02 |
| Status | Retired December 1, 2025 |
| Level | Specialty |
| Purpose | Validate advanced AWS security knowledge and skills |
| Target candidate | Experienced AWS security practitioners |
| Prerequisites | No formal prerequisite |
| Duration | 170 minutes |
| Questions | 65 scored/unscored questions |
| Format | Multiple choice and multiple response |
| Passing score | 750/1000 |
| Delivery | Pearson VUE testing center or online proctored |

AWS described the target candidate as someone with substantial IT security experience and hands-on experience securing AWS workloads. :contentReference[oaicite:0]{index=0}

## Who Should Take It?

For the historical SCS-C02 exam, the ideal learner had practical AWS experience and a strong foundation in cloud security, IAM, networking, encryption, monitoring, logging, and incident response.

AWS recommended significant security and AWS workload experience rather than treating this as a beginner certification. :contentReference[oaicite:1]{index=1}

## Exam Objectives / Domains

SCS-C02 covered major AWS security responsibilities including:

- **Incident Response** — Prepare for, detect, investigate, and respond to security events.
- **Logging and Monitoring** — Use CloudTrail, CloudWatch, security findings, centralized logging, and monitoring mechanisms.
- **Infrastructure Security** — Secure VPCs, network traffic, compute workloads, edge services, and application infrastructure.
- **Identity and Access Management** — Design IAM policies, roles, federation, authentication, authorization, and least-privilege access.
- **Data Protection** — Protect data at rest and in transit using encryption, KMS, certificates, secrets, and appropriate controls.
- **Management and Security Governance** — Apply security controls across AWS accounts, organizations, compliance requirements, and governance processes.

Because SCS-C02 is retired, candidates studying for the current certification should use the SCS-C03 objectives instead. AWS's current exam guide uses six domains: Detection, Incident Response, Infrastructure Security, Identity and Access Management, Data Protection, and Security Foundations and Governance. :contentReference[oaicite:2]{index=2}

## Detailed Study Notes

### IAM and Identity

Understand IAM users, groups, roles, policies, policy evaluation, resource-based policies, federation, temporary credentials, MFA, and least privilege.

**Example:** Prefer an IAM role with temporary credentials for an EC2 workload instead of embedding long-term access keys in application code.

### Detection and Logging

Understand CloudTrail management/data events, CloudWatch monitoring, centralized logging, GuardDuty findings, and Security Hub aggregation.

Know why logs should be protected from unauthorized modification and how organizations can centralize security visibility.

### Network Security

Study VPC security groups, network ACLs, routing, private/public subnets, VPC endpoints, AWS WAF, AWS Shield, TLS, and network segmentation.

A security group is stateful; network ACLs operate at the subnet level and are stateless.

### Encryption and Key Management

Understand AWS KMS keys, key policies, grants, encryption at rest, TLS encryption in transit, envelope encryption, and key rotation concepts.

Never place secrets directly in source code. Use appropriate AWS secret-management mechanisms.

### Incident Response

Build a repeatable process for detecting, containing, investigating, and recovering from security incidents.

Useful AWS capabilities include CloudTrail, GuardDuty, Security Hub, IAM, EC2, S3, and AWS Organizations.

### Data Protection

Study S3 encryption and bucket policies, EBS encryption, database encryption, TLS certificates, Secrets Manager, Systems Manager Parameter Store, and KMS.

Always match the security control to the data classification and threat model.

## Important Concepts

- Shared responsibility model
- Least privilege
- IAM policy evaluation
- IAM roles and temporary credentials
- MFA and federation
- AWS Organizations and SCPs
- CloudTrail
- CloudWatch
- GuardDuty
- Security Hub
- AWS Config
- AWS WAF and Shield
- VPC security groups and NACLs
- KMS and envelope encryption
- Secrets Manager
- S3 security
- TLS
- Incident response
- Centralized security logging
- Compliance and governance

## Practical Examples / Labs

Use a personal AWS account or approved training environment and:

1. Create an IAM role for an EC2 workload.
2. Test least-privilege IAM policies.
3. Enable CloudTrail and review events.
4. Configure CloudWatch security monitoring.
5. Explore GuardDuty findings.
6. Create secure S3 bucket policies and encryption settings.
7. Encrypt an EBS volume using KMS.
8. Store application credentials in Secrets Manager.
9. Build a VPC with public/private segmentation.
10. Configure AWS WAF rules in a controlled test environment.

Avoid testing security controls against systems you do not own or have permission to assess.

## Study Strategy

Start with the official AWS exam guide and documentation. Learn the purpose and security trade-offs of each service instead of memorizing service names.

Combine:

1. AWS documentation and exam objectives.
2. Hands-on labs.
3. Architecture diagrams.
4. Legitimate AWS practice questions.
5. Review of incorrect answers.
6. Repeated revision of IAM, networking, encryption, logging, and incident response.

AWS states that practical experience is an important part of preparation for Specialty certifications. :contentReference[oaicite:3]{index=3}

## 30-Day Study Plan

- **Days 1–4:** AWS security fundamentals and shared responsibility.
- **Days 5–8:** IAM, roles, policies, federation, and MFA.
- **Days 9–12:** CloudTrail, CloudWatch, GuardDuty, Security Hub, and Config.
- **Days 13–16:** VPC, security groups, NACLs, WAF, Shield, and network security.
- **Days 17–20:** KMS, encryption, S3, EBS, databases, and secrets.
- **Days 21–23:** Incident response and forensic concepts.
- **Days 24–25:** Organizations, SCPs, governance, and compliance.
- **Days 26–27:** Hands-on revision.
- **Day 28:** Legitimate practice assessment.
- **Day 29:** Review weak areas.
- **Day 30:** Final revision and objective-by-objective checklist.

## Common Mistakes

- Memorizing AWS services without understanding use cases.
- Giving excessive permissions instead of applying least privilege.
- Confusing security groups with network ACLs.
- Storing credentials in application source code.
- Ignoring encryption key-management requirements.
- Treating logging as optional.
- Using outdated SCS-C02 objectives for the current SCS-C03 exam.
- Using dumps, leaked questions, or unauthorized recalled questions.

## Exam-Day Tips

For historical SCS-C02 preparation, read each scenario carefully and identify the security requirement first. Eliminate options that violate least privilege, introduce unnecessary operational complexity, or fail the stated security objective.

Manage time across the full exam and flag uncertain questions for later review where the testing interface permits.

## Final Checklist

- [ ] Understand IAM policy evaluation.
- [ ] Know common AWS security services.
- [ ] Understand VPC security controls.
- [ ] Review KMS and encryption.
- [ ] Practice CloudTrail and monitoring concepts.
- [ ] Understand incident-response workflows.
- [ ] Review governance and compliance.
- [ ] Confirm whether you actually need SCS-C03 instead of retired SCS-C02.

## Official Resources

- [AWS Certified Security - Specialty](https://aws.amazon.com/certification/certified-security-specialty/)
- [AWS Certification Exam Guides](https://docs.aws.amazon.com/aws-certification/latest/examguides/aws-certification-exam-guides.html)
- [SCS-C03 current exam guide](https://docs.aws.amazon.com/aws-certification/latest/security-specialty-03/security-specialty-03.html)
- [SCS-C02 vs. SCS-C03 comparison](https://docs.aws.amazon.com/aws-certification/latest/security-specialty-03/security-specialty-03-appendix-b.html)
- [AWS Skill Builder](https://skillbuilder.aws/)
- [AWS Documentation](https://docs.aws.amazon.com/)

AWS confirms that SCS-C02 was replaced by SCS-C03 beginning December 2, 2025. :contentReference[oaicite:4]{index=4}

## Voucher / Discount

Learn SecByte provides certification voucher options and discounts where available.

**SCS-C02 is retired**, so candidates should verify voucher validity and current AWS exam availability before purchasing. For current AWS Security Specialty certification preparation, check whether an SCS-C03 voucher is appropriate.

Voucher URL:

https://learn.secbyte.org/vouchers/aws-scs-c02

## Disclaimer

This is an independent/community study guide and is not affiliated with or endorsed by AWS. AWS, Amazon Web Services, and related names are trademarks of Amazon.com, Inc. or its affiliates. Certification information can change, so verify current details with AWS. Voucher pricing and availability may change. This repository contains no exam dumps, leaked questions, or recalled exam questions.
