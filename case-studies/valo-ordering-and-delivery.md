# VALO Systems ordering and delivery

**Implementation summary · Business applications · Part-time venture**

I build business applications through VALO Systems alongside my full-time engineering role. The work includes gas ordering and delivery software, a multi-tenant SHEQ platform, and release automation for AWS and cPanel.

This summary describes implementation work without publishing client code, customer messages or operational data. It does not claim a currently available public demo.

## From a WhatsApp message to a reviewed order

Order requests arrive as free text, while an ordering system needs structured fields. I built an AWS Bedrock workflow to extract proposed order details and prefill an order for an operator to review.

1. Receive the message as input to the ordering workflow.
2. Extract a structured proposal using Bedrock.
3. Validate the schema and carry confidence and ambiguity fields into review.
4. Let the operator check and complete the proposed order before it enters the normal ordering process.
5. Fall back to manual entry when extraction times out or cannot provide usable fields.

The model assists capture. Operator review remains part of the workflow, and a model-provided confidence field is not a measured accuracy guarantee.

## Applications and delivery

Across the gas ordering and SHEQ projects, I have used React, TypeScript, Node.js, Java/Spring Boot, PostgreSQL and AWS. My contribution spans requirements, application development, integrations, infrastructure and deployment.

I also built GitHub Actions pipelines for AWS and Git-based cPanel releases. The pipelines cover automated checks, release packaging, deployment gates and health verification, with Terraform used for cloud infrastructure.

## Engineering decisions

- **Keep an editable proposal:** free-text extraction helps the operator without silently turning an ambiguous message into a completed order.
- **Validate the handoff:** schema checks and explicit ambiguity fields make incomplete extraction visible.
- **Provide a manual path:** timeouts and unusable output should leave an operator able to continue.
- **Make releases repeatable:** build, package, deploy and verify through a defined pipeline.

## Evidence and boundaries

The public summary establishes what I worked on; it does not substitute for access to the implementation or a current service demonstration. It contains no customer adoption, throughput, accuracy or revenue claim.

For source code and reproducible engineering evidence available without client access, start with my [Fraud Rule Engine case study](https://github.com/SibusisoMashita/fraud-rule-engine-service/blob/main/docs/CASE_STUDY.md).

[Back to my GitHub profile](../README.md)
