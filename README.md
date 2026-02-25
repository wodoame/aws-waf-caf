# AWS Well-Architected & Cloud Adoption Assessment

This repository contains my comprehensive evaluation and redesigned architecture for migrating a two-tier web application (frontend + backend database) from on-premises servers to the AWS Cloud. My goal for this project is to ensure the migration aligns with AWS best practices from day one.

## Project Overview

My migration strategy focuses on moving away from a high-risk, single-AZ on-premises environment toward a resilient, scalable, and secure AWS infrastructure. In this project, I utilize two primary AWS frameworks:

1. **AWS Well-Architected Framework (WAF):** I use this to evaluate and improve the workload across five pillars: Operational Excellence, Security, Reliability, Performance Efficiency, and Cost Optimization.
2. **AWS Cloud Adoption Framework (CAF):** I use this to analyze organizational readiness across Business, People, Governance, Platform, Security, and Operations perspectives.

## Repository Structure

* `aws_waf_caf_assessment.md`: My primary report containing the WAF assessment table and CAF readiness summary.
* `architecture_diagram.png`: A visual representation of my improved Multi-AZ AWS architecture.
* `README.md`: This file, explaining my project approach and objectives.

## Technical Approach

### 1. Risk Identification

I identified several critical weaknesses in the initial on-premises architecture:

* **Single-AZ Deployment:** Lack of high availability.
* **Security Gaps:** Open security groups and lack of encryption.
* **Manual Operations:** No automated backup or deployment strategy.

### 2. Well-Architected Improvements

My proposed design addresses these risks by implementing:

* **Multi-AZ Availability:** Using an Application Load Balancer (ALB) and Auto Scaling Groups.
* **Data Persistence:** Migrating the database to Amazon RDS (Multi-AZ) for automated backups and failover.
* **Infrastructure as Code:** Leveraging AWS CloudFormation or CDK for consistent deployments.

### 3. Cloud Adoption Readiness

My CAF assessment highlights the need for a shift in organizational culture, specifically moving from fixed capital expenses (CapEx) to variable operational expenses (OpEx) and adopting a "security-by-design" mindset.

## Deliverables

* **Task 2:** Completed WAF Assessment Table.
* **Task 3:** CAF Readiness Summary.
* **Task 4:** Improved Architecture Description and Diagram.
* **Reflection:** A brief summary of my learning outcomes.
