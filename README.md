# Sibusiso Mashita

**Senior software engineer · Backend services, payments and cloud delivery**

I’m a South African software engineer building backend services and complete business applications. My core stack is Java, Spring Boot and AWS, supported by substantial C#/.NET experience and React/TypeScript product development.

At Capitec, I work on payment services and AWS integrations. Alongside that role, I run VALO Systems part-time, building business applications and release pipelines from requirements through deployment.

[LinkedIn](https://www.linkedin.com/in/sibusisomashita/) · [VALO Systems](https://github.com/valo-systems) · **Open to fully remote engineering opportunities**

## Selected work

### Fraud Rule Engine
**Flagship engineering case study · Technical assessment with synthetic data**

A Java 21/Spring Boot service and React/TypeScript interface for evaluating booked transactions against configurable fraud rules. The work focuses on transaction safety, explainable decisions, replay handling and policy changes that preserve earlier results.

- **One complete record:** event, evaluation and rule evidence commit together.
- **Explicit recovery:** an identical replay returns the saved decision; conflicting content is rejected; uncertain writes keep their original identity.
- **Traceable policy:** each evaluation retains the policy version and evidence used to make it.

[Read the case study](https://github.com/SibusisoMashita/fraud-rule-engine-service/blob/main/docs/CASE_STUDY.md) · [Backend](https://github.com/SibusisoMashita/fraud-rule-engine-service) · [Interface](https://github.com/SibusisoMashita/fraud-rule-engine-ui) · [Verification evidence](https://github.com/SibusisoMashita/fraud-rule-engine-service/blob/main/docs/TESTING.md)

### VALO Systems
**Business application development · Part-time venture**

Gas ordering and delivery software, a multi-tenant SHEQ platform, and GitHub Actions pipelines for AWS and cPanel. An AI-assisted ordering workflow extracts details from WhatsApp messages, validates the proposed fields and prefills an order for an operator to review.

[Read the implementation summary](case-studies/valo-ordering-and-delivery.md) · [VALO organization](https://github.com/valo-systems)

### FixSA Voice
**Voice product prototype · AssemblyAI hackathon demonstration**

A Next.js/Laravel civic reporting prototype exploring voice-led report capture and resident verification of a claimed repair. The demonstration uses synthetic data and has no municipal or emergency-service integration.

[Explore the project](https://github.com/SibusisoMashita/fixsa-voice) · [Recorded walkthrough](https://github.com/SibusisoMashita/fixsa-voice/releases/download/v1.0.0-hackathon/FixSA-Voice-Demo.mp4)

### Earlier work: Vault Vibes
**Archived prototype · Financial domain modelling**

A Spring Boot and React exploration of stokvel contributions, loans and member dashboards, with AWS/Cognito integration. Retained as an earlier prototype; the repositories are archived and are not presented as a production financial service.

[Backend](https://github.com/SibusisoMashita/vault-vibes-backend) · [Frontend](https://github.com/SibusisoMashita/vault-vibes-frontend)

## How I work

| Area | Tools and focus |
| --- | --- |
| Backend | Java, Spring Boot, C#/.NET, Node.js, TypeScript, REST APIs |
| Data and integration | PostgreSQL, SQL Server, MySQL, DynamoDB, SQS and SNS |
| Delivery | AWS, Docker, EKS, ArgoCD, Terraform, GitHub Actions and cPanel |
| Product development | React, business workflows and AI-assisted data capture |

I make failure paths visible, keep business decisions traceable and check behaviour across the application and its dependencies. The repositories above include the implementation, setup instructions, tests and remaining limitations so reviewers can inspect the work.

These public projects are separate from my employer’s production systems. Assessment and prototype evidence describes its documented scope; it does not establish production banking use or business impact.
