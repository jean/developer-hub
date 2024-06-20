---
title: CD Best Practices
description: Best Practices for Harness CD & GitOps
sidebar_position: 3
---

This topic will detail best practices for using Harness CD and GitOps.

## Don't Repeat Yourself

Keep your pipelines DRY! DRY is an acronym used in software development that stands for Don't Repeat Yourself. It emphasizes the importance of avoiding redundancy to make the codebase easier to understand, maintain, and less prone to errors. For CI/CD pipelines, particularly in Harness, it is essential to have a DRY approach for efficiency and consistency.

For a guide on how to do so, go to [Keep Your Pipelines DRY](/docs/continuous-delivery/cd-onboarding/new-user/rampup-dry)

## Use permissions and RBAC (Role Based Access Control)

Make sure to control which environments developers or users can access for deployments in order to ensure security and avoid accidents. 

To learn more, go to [Access Control for Environments](/docs/continuous-delivery/cd-onboarding/existing-user/prevent-devs-deploying-higher-env)

## Services

### Don't map one Harness Service to multiple micro services. 

A [Harness Service](/docs/continuous-delivery/get-started/key-concepts#service) is a logical construct used to represent a microservice or workload. Therefore, ensure that your Harness Service is associated with or represents exactly one microservice or workload. 

Do not be afraid to create more services. 