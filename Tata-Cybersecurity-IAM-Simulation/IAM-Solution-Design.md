# IAM Solution Design

## Task Overview

In this task, I designed IAM solutions for TechCorp based on the issues identified during the readiness assessment.

The two main focus areas were:

- User lifecycle management
- Access control mechanisms

## User Lifecycle Management

I proposed an automated Joiner-Mover-Leaver process.

### Joiner
When a new employee joins TechCorp, their account and required access should be created automatically based on information from the HR system.

### Mover
When an employee changes role or department, their permissions should be updated so that old access is removed and new access is granted.

### Leaver
When an employee leaves the organisation, their accounts and access should be disabled or removed promptly.

This process helps reduce manual errors and prevents users from keeping access they no longer need.

## Access Control

I proposed Role-Based Access Control (RBAC) so that users receive permissions based on their job responsibilities.

I also considered the following controls:

- Principle of Least Privilege
- Multi-Factor Authentication (MFA)
- Single Sign-On (SSO)
- Regular access reviews
- Privileged account monitoring

## Technologies Considered

The simulation introduced technologies such as:

- SailPoint for identity lifecycle management
- Oracle Identity Manager for role-based access management
- Active Directory integration
- HR system integration using connectors or APIs

These technologies were proposed as part of the solution design and were not personally deployed or configured during the simulation.

## Why These Controls Matter

Automated user lifecycle management can reduce delays and errors during onboarding, role changes, and offboarding.

RBAC and least privilege help ensure that users only receive the access they need.

MFA adds an extra layer of protection against stolen passwords, while SSO can improve the user experience by reducing the number of separate logins.

## What I Learned

This task helped me understand how cybersecurity professionals move from identifying a security problem to selecting an appropriate IAM control.

I learned to think in the following way:

**Business Problem → Security Risk → IAM Control → Business Benefit**

For example:

- Former employee account remains active
- Risk of unauthorised access
- Automated deprovisioning
- Reduced security risk

## SOC Relevance

IAM controls are important in SOC environments because identity-related activity can be an indicator of compromise.

Examples include:

- Suspicious login attempts
- Unexpected privilege changes
- Unusual account activity
- Access from unauthorised users
- Compromised credentials

Understanding access control helps a SOC analyst determine whether account activity is normal or suspicious.
