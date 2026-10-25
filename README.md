```{=html}
<!--
Professional Cloud / DevSecOps profile README
Primary focus: Microsoft Azure, Terraform, DevSecOps, Platform Engineering and GenAI-assisted automation.
-->
```
::: {align="center"}
`<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0A0E27,40:0078D4,100:8A2BE2&height=280&section=header&text=GUNJAN%20KUMAR%20GAURAV&fontSize=52&fontColor=FFFFFF&fontAlignY=38&desc=Senior%20Cloud%20%7C%20DevSecOps%20%7C%20GenAI%20Consultant&descAlignY=58&descSize=20&animation=fadeIn" width="100%"/>`{=html}

### Senior Cloud, DevSecOps & GenAI Consultant

**Microsoft Azure · Terraform · Azure DevOps · GitHub Actions ·
DevSecOps · Cloud Security · Platform Engineering**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-0078D4?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/gunjan-gaurav)
[![GitHub](https://img.shields.io/badge/GitHub-0A0E27?style=for-the-badge&logo=github&logoColor=white)](https://github.com/gunjankumargaurav7350)
:::

------------------------------------------------------------------------

## `$ whoami`

``` text
NAME        : Gunjan Kumar Gaurav
ROLE        : Senior Cloud, DevSecOps & GenAI Consultant
LOCATION    : India
SPECIALTY   : Microsoft Azure | Terraform | DevSecOps | Platform Engineering
MISSION     : Build secure, scalable, observable and automated cloud platforms.
ENGINEERING : Infrastructure as Code + CI/CD + Security + Governance + Automation
```

> Infrastructure should be repeatable. Security should be automated.
> Operations should be observable. Cloud architecture should be built to
> scale.

## 📚 Table of Contents

-   [Professional Profile](#professional-profile)
-   [Engineering Philosophy](#engineering-philosophy)
-   [Technical Arsenal](#technical-arsenal)
-   [Azure Architecture](#azure-architecture)
-   [Azure Landing Zones](#azure-landing-zones)
-   [Azure Governance](#azure-governance)
-   [Azure Networking](#azure-networking)
-   [Identity and Access Management](#identity-and-access-management)
-   [Azure Security](#azure-security)
-   [Azure Compute](#azure-compute)
-   [Azure Storage](#azure-storage)
-   [Azure Database](#azure-database)
-   [Azure Monitoring and
    Observability](#azure-monitoring-and-observability)
-   [Terraform Engineering](#terraform-engineering)
-   [Terraform Modules](#terraform-modules)
-   [Terraform State](#terraform-state)
-   [Terraform Security](#terraform-security)
-   [Terraform CI/CD](#terraform-cicd)
-   [Azure DevOps](#azure-devops)
-   [GitHub Actions](#github-actions)
-   [DevSecOps](#devsecops)
-   [Policy as Code](#policy-as-code)
-   [Secret Management](#secret-management)
-   [Container and Kubernetes
    Security](#container-and-kubernetes-security)
-   [Networking Security Patterns](#networking-security-patterns)
-   [Observability Engineering](#observability-engineering)
-   [FinOps and Cost Optimization](#finops-and-cost-optimization)
-   [Reliability and Disaster
    Recovery](#reliability-and-disaster-recovery)
-   [Platform Engineering](#platform-engineering)
-   [GenAI for Cloud Engineering](#genai-for-cloud-engineering)
-   [Enterprise Delivery Workflow](#enterprise-delivery-workflow)
-   [Project Portfolio](#project-portfolio)
-   [Operational Runbooks](#operational-runbooks)
-   [Security Checklists](#security-checklists)
-   [Terraform Command Reference](#terraform-command-reference)
-   [Azure CLI Reference](#azure-cli-reference)
-   [Git Reference](#git-reference)
-   [PowerShell Reference](#powershell-reference)
-   [Bash Reference](#bash-reference)
-   [Interview-Level Architecture
    Questions](#interview-level-architecture-questions)
-   [Current Focus](#current-focus)
-   [Certifications](#certifications)
-   [Engineering Principles](#engineering-principles)

# Professional Profile

## Professional Profile

The engineering focus represented in this profile is centered on
designing and operating Azure environments where infrastructure,
delivery, security and governance are treated as one system.

### Core outcomes

-   Standardize Azure infrastructure through reusable Terraform modules.
-   Reduce configuration drift through declarative Infrastructure as
    Code.
-   Move security controls into pull requests and CI/CD rather than
    relying only on runtime review.
-   Separate platform foundations from application workloads.
-   Use Azure governance controls to establish organization-wide
    guardrails.
-   Design network boundaries before deploying workloads.
-   Prefer identity-based authentication over long-lived credentials.
-   Keep Terraform state remote, protected and recoverable.
-   Make production changes auditable and reviewable.
-   Build observability into the platform instead of adding it after
    incidents.
-   Treat cloud cost as an engineering signal, not only a finance
    report.
-   Automate repeatable operational tasks with PowerShell, Bash and
    CI/CD.
-   Use GenAI as an engineering accelerator while retaining human
    approval for high-impact changes.

### Engineering scope

  -----------------------------------------------------------------------
  Domain                              Primary focus
  ----------------------------------- -----------------------------------
  Cloud                               Microsoft Azure

  IaC                                 Terraform, Bicep, ARM Templates

  CI/CD                               Azure DevOps, GitHub Actions

  Security                            Checkov, tfsec, TFLint, TruffleHog,
                                      Trivy

  Testing                             Terraform validation, Terratest

  Networking                          VNet, subnet, NSG, peering,
                                      firewall, private endpoints

  Identity                            RBAC, PIM, managed identity, Key
                                      Vault

  Governance                          Management Groups, Azure Policy,
                                      Landing Zones

  Observability                       Azure Monitor, Log Analytics,
                                      Grafana, Nagios, Zabbix

  FinOps                              Infracost, OpenCost, rightsizing
                                      and governance

  Automation                          PowerShell, Bash, Python

  Platform                            Reusable modules, standards, golden
                                      paths

  AI                                  GenAI-assisted infrastructure
                                      review and automation
  -----------------------------------------------------------------------

# Engineering Philosophy

## Engineering Philosophy

### 1. Infrastructure as Code first

If an infrastructure component matters to production, its desired
configuration should be represented as code whenever practical.

The repository becomes the review surface for:

-   infrastructure intent
-   dependency relationships
-   security controls
-   configuration standards
-   deployment history
-   rollback information
-   ownership boundaries

### 2. Secure by design

Security is not a final pipeline stage.

Security requirements should influence:

1.  identity
2.  network topology
3.  data protection
4.  secret handling
5.  infrastructure code
6.  CI/CD controls
7.  runtime monitoring
8.  incident response

### 3. Least privilege

Every identity should receive only the permissions required for its
responsibility.

Prefer:

-   managed identities
-   workload identity federation
-   scoped RBAC
-   PIM for privileged access
-   Key Vault for secrets

Avoid:

-   hard-coded credentials
-   broad Owner assignments
-   shared administrator accounts
-   permanent privileged access
-   secrets committed to repositories

### 4. Immutable and repeatable delivery

The preferred workflow is:

``` text
Developer
   |
   v
Pull Request
   |
   +--> Format / Validate
   |
   +--> Lint
   |
   +--> Security Scan
   |
   +--> Secret Scan
   |
   +--> Cost Estimate
   |
   +--> Terraform Plan
   |
   v
Approval
   |
   v
Terraform Apply
   |
   v
Monitoring / Audit / Drift Detection
```

### 5. Operational visibility

A successful deployment is not the end of delivery.

The platform should answer:

-   Is the service healthy?
-   Is the infrastructure reachable?
-   Are error rates increasing?
-   Are latency and saturation changing?
-   Is a security control failing?
-   Did the deployment create unexpected cost?
-   Is infrastructure drifting from the declared state?

# Technical Arsenal

## Technical Arsenal

### ☁️ Microsoft Azure

-   Azure Resource Groups
-   Azure Subscriptions
-   Azure Management Groups
-   Azure Policy
-   Azure RBAC
-   Microsoft Entra ID
-   Azure Key Vault
-   Azure Virtual Network
-   Azure Subnets
-   Network Security Groups
-   Azure Load Balancer
-   Azure Application Gateway
-   Azure Bastion
-   Azure Firewall
-   Private Endpoints
-   Private DNS
-   VNet Peering
-   Azure Virtual WAN
-   Azure Monitor
-   Log Analytics
-   Microsoft Defender for Cloud
-   Microsoft Sentinel
-   Azure Storage
-   Azure Virtual Machines
-   Azure Kubernetes Service
-   Azure Database services
-   Azure Advisor
-   Azure Migrate

### 🏗️ Infrastructure as Code

-   Terraform
-   Terraform modules
-   Terraform variables
-   Terraform locals
-   Terraform outputs
-   Terraform data sources
-   `for_each`
-   `count`
-   `depends_on`
-   `lifecycle`
-   remote state
-   state locking
-   provider version constraints
-   provider aliases
-   reusable module contracts
-   Terraform plan review
-   Terraform import
-   drift analysis

### 🔁 Delivery

-   Azure DevOps Pipelines
-   Azure Repos
-   Azure service connections
-   GitHub Actions
-   YAML pipelines
-   pull-request validation
-   branch protection
-   manual approvals
-   environment gates
-   artifact promotion
-   blue-green deployment
-   canary deployment
-   rolling deployment
-   GitFlow

### 🛡️ DevSecOps

-   Checkov
-   tfsec
-   TFLint
-   TruffleHog
-   Trivy
-   Terratest
-   SonarQube
-   policy-as-code
-   secret scanning
-   IaC security
-   container security
-   dependency security
-   least privilege
-   secure CI/CD

### 📊 Observability

-   Azure Monitor
-   Log Analytics
-   Grafana
-   Nagios
-   Zabbix
-   OpenCost
-   Infracost
-   metrics
-   logs
-   traces
-   alerting
-   dashboards
-   SLO/SLA-oriented monitoring

### 💻 Automation

-   PowerShell
-   Bash
-   Python
-   Azure CLI
-   Git
-   REST APIs
-   YAML

# Azure Architecture

## Azure Architecture

### Architecture principles

A production Azure platform should establish clear separation between:

-   management plane
-   identity plane
-   connectivity plane
-   security plane
-   shared services
-   application landing zones
-   observability
-   governance
-   cost management

### Reference topology

``` text
                    ┌──────────────────────────┐
                    │     Microsoft Entra ID   │
                    │ Identity / RBAC / PIM    │
                    └────────────┬─────────────┘
                                 |
                    ┌────────────v─────────────┐
                    │   Management Groups      │
                    │ Governance / Policy      │
                    └────────────┬─────────────┘
                                 |
          ┌──────────────────────v──────────────────────┐
          │              Connectivity Hub               │
          │ Firewall | DNS | Bastion | Gateway | VPN   │
          └───────────────┬───────────────┬─────────────┘
                          |               |
                 ┌────────v──────┐ ┌─────v────────────┐
                 │ Production    │ │ Non-Production   │
                 │ Landing Zone  │ │ Landing Zone     │
                 └────────┬──────┘ └─────┬────────────┘
                          |               |
                    ┌─────v────────────────v─────┐
                    │ Application Workloads      │
                    │ VM | AKS | App Services   │
                    └────────────────────────────┘
```

### Control-plane separation

The platform should distinguish:

-   who can create resources
-   who can change network boundaries
-   who can administer identities
-   who can deploy workloads
-   who can read secrets
-   who can approve production changes
-   who can investigate security incidents

### Subscription strategy

A subscription boundary can be used for:

-   billing separation
-   workload isolation
-   policy scope
-   quota management
-   blast-radius reduction
-   delegated administration
-   environment separation

Subscription design should follow organizational requirements rather
than arbitrary subscription proliferation.

### Naming

A consistent naming convention should encode useful context without
making names excessively long.

Example:

``` text
<resource-type>-<workload>-<environment>-<region>-<instance>
```

Example:

``` text
rg-platform-prod-centralindia
vnet-app-prod-centralindia
kv-app-prod-centralindia
```

### Tagging

Recommended governance tags include:

-   `Environment`
-   `Application`
-   `Owner`
-   `CostCenter`
-   `BusinessUnit`
-   `ManagedBy`
-   `DataClassification`
-   `Criticality`

Tags should be governed centrally where organizational policy requires
them.

# Azure Landing Zones

## Azure Landing Zones

An Azure Landing Zone is a standardized platform foundation that gives
workload teams a governed place to deploy applications.

### Core building blocks

1.  Tenant and identity foundation
2.  Management group hierarchy
3.  Subscription vending
4.  Connectivity
5.  Security
6.  Governance
7.  Operations
8.  Application landing zones

### Management group hierarchy

A conceptual structure can look like:

``` text
Tenant Root
|
+-- Platform
|   +-- Connectivity
|   +-- Identity
|   +-- Management
|   +-- Security
|
+-- Landing Zones
|   +-- Production
|   +-- NonProduction
|
+-- Sandbox
|
+-- Decommissioned
```

### Governance flow

``` text
Management Group
      |
      v
Policy Assignment
      |
      v
Subscription
      |
      v
Resource Group
      |
      v
Resource
```

### Landing zone guardrails

Typical guardrails include:

-   allowed Azure regions
-   required tags
-   diagnostic settings
-   encryption requirements
-   private networking requirements
-   public IP restrictions
-   resource SKU restrictions
-   Defender coverage
-   identity requirements
-   naming conventions
-   approved resource types

### Workload onboarding

A workload should provide:

-   owner
-   business criticality
-   data classification
-   network requirements
-   identity requirements
-   backup requirements
-   monitoring requirements
-   RTO
-   RPO
-   expected traffic
-   expected cost

### Landing zone acceptance criteria

``` text
[ ] Subscription created
[ ] Correct management group assigned
[ ] Required policies inherited
[ ] RBAC model approved
[ ] Connectivity available
[ ] DNS resolution verified
[ ] Logging enabled
[ ] Security baseline enabled
[ ] Backup requirements defined
[ ] Cost tags applied
[ ] CI/CD identity configured
[ ] Terraform state secured
```

# Azure Governance

## Azure Governance

### Management Groups

Management Groups provide a hierarchy above subscriptions and allow
governance to be applied at scale.

Use them to organize:

-   policy scope
-   RBAC boundaries
-   subscription hierarchy
-   enterprise governance

### Azure Policy

Azure Policy evaluates resources against organizational rules.

Common policy effects include:

-   Audit
-   Deny
-   Modify
-   DeployIfNotExists

A mature governance model should distinguish between:

-   mandatory controls
-   remediation controls
-   advisory controls
-   temporary exemptions

### Policy exemption

An exemption should be:

-   justified
-   scoped
-   owned
-   time-bound where possible
-   documented
-   reviewed

### RBAC

Azure RBAC is based on:

``` text
Security Principal
        +
Role Definition
        +
Scope
        =
Effective Access
```

Scopes can be:

-   management group
-   subscription
-   resource group
-   resource

### PIM

Privileged Identity Management reduces standing privileged access.

A strong model uses:

-   eligible access
-   approval
-   time-bound activation
-   MFA
-   justification
-   audit logs

### Governance anti-patterns

Avoid:

-   one subscription for everything
-   everyone as Owner
-   permanent admin accounts
-   policies that nobody understands
-   unlimited policy exemptions
-   missing resource ownership
-   unmanaged public endpoints
-   inconsistent tagging

### Governance maturity

``` text
Level 1  Manual controls
Level 2  Documented standards
Level 3  Policy enforcement
Level 4  Automated remediation
Level 5  Continuous compliance and optimization
```

# Azure Networking

## Azure Networking

### VNet fundamentals

A Virtual Network provides the private network boundary for Azure
workloads.

Core concepts:

-   address space
-   subnet
-   route
-   NSG
-   DNS
-   peering
-   private endpoint
-   gateway
-   firewall

### Subnet design

Do not create subnets only because a diagram looks clean.

Create boundaries based on:

-   security requirements
-   routing requirements
-   workload role
-   delegated services
-   operational ownership

Example:

``` text
VNet: 10.10.0.0/16

10.10.1.0/24   App Gateway
10.10.2.0/24   Application
10.10.3.0/24   Data
10.10.4.0/24   Private Endpoints
10.10.5.0/24   Management / Bastion
```

### NSG

A Network Security Group controls network traffic using rules.

Rule evaluation should be designed deliberately around:

-   source
-   destination
-   port
-   protocol
-   direction
-   priority
-   allow/deny

### Hub and spoke

The hub provides shared network capabilities.

Spokes isolate workload networks.

``` text
                    HUB
        ┌────────────┼────────────┐
        │            │            │
     Firewall      DNS         Bastion
        │
   ┌────┴─────┐
   │          │
Spoke-App   Spoke-Data
```

### VNet Peering

VNet peering provides private connectivity between VNets.

Validate:

-   address spaces do not overlap
-   required forwarding is enabled
-   route tables are correct
-   NSGs permit the flow
-   firewall paths are understood

### Private Endpoint

A Private Endpoint maps a PaaS service into a VNet through a private IP.

Operational considerations:

-   private DNS
-   DNS zone links
-   subnet policy
-   NSGs
-   routing
-   name resolution

### Azure Firewall

Use centralized firewalling when the architecture requires:

-   controlled egress
-   centralized inspection
-   network segmentation
-   application rules
-   network rules
-   threat intelligence

### Azure Bastion

Bastion provides browser-based secure access to supported VMs without
exposing management ports directly to the internet.

### Application Gateway and WAF

Application Gateway provides Layer 7 traffic management.

WAF adds web application protection capabilities.

Typical flow:

``` text
Internet
   |
   v
Application Gateway / WAF
   |
   v
Application subnet
   |
   v
Backend workload
```

### Network troubleshooting sequence

``` text
1. DNS resolution
2. Route table
3. NSG
4. Firewall
5. Peering
6. Private endpoint
7. Service endpoint
8. Application listener
9. Backend health
10. Application logs
```

# Identity and Access Management

## Identity and Access Management

### Microsoft Entra ID

Identity should be the primary control plane for authentication and
authorization.

Core concepts:

-   users
-   groups
-   service principals
-   managed identities
-   workload identities
-   applications
-   service connections

### Managed Identity

Managed identity removes the need to distribute credentials to supported
Azure resources.

Conceptual flow:

``` text
Azure Workload
      |
      v
Managed Identity
      |
      v
Microsoft Entra ID
      |
      v
Azure Resource
```

### System-assigned identity

The lifecycle is tied to the Azure resource.

### User-assigned identity

The identity is an independent Azure resource and can be associated with
multiple supported resources.

### RBAC design

A role assignment should answer:

-   Who?
-   What role?
-   At what scope?
-   For how long?
-   Why?

### CI/CD authentication

Preferred enterprise patterns include:

-   workload identity federation
-   managed identity where applicable
-   tightly scoped service connections

Avoid putting:

-   client secrets
-   passwords
-   access keys

inside YAML files.

### Access review

Periodic access reviews should identify:

-   unused assignments
-   broad assignments
-   stale service principals
-   excessive privileges
-   permanent privileged access

### Zero Trust

Zero Trust is based on:

-   verify explicitly
-   use least privilege
-   assume breach

Architecture implications:

-   authenticate every workload
-   minimize network trust
-   isolate identities
-   protect data
-   monitor anomalous access

# Azure Security

## Azure Security

### Defense in depth

Use multiple independent security layers:

``` text
Identity
   |
Network
   |
Application
   |
Data
   |
Monitoring
   |
Response
```

### Key Vault

Use Key Vault for supported:

-   secrets
-   keys
-   certificates

Design for:

-   RBAC
-   private connectivity where required
-   logging
-   soft-delete
-   purge protection where appropriate
-   managed identity access

### Defender for Cloud

Use Defender for Cloud for security posture and workload protection
capabilities appropriate to the environment.

### Microsoft Sentinel

Sentinel can provide:

-   security analytics
-   incident management
-   threat detection
-   investigation
-   automation

### Secret scanning

A DevSecOps pipeline should detect accidental credential exposure before
merge.

Tools can include:

-   TruffleHog
-   repository secret scanning
-   provider-specific secret detectors

### IaC scanning

Terraform should be scanned for:

-   public exposure
-   weak encryption
-   missing logging
-   overly broad permissions
-   insecure network configuration
-   missing security controls

### Security gates

A practical pipeline:

``` text
Terraform fmt
   |
Terraform validate
   |
TFLint
   |
Checkov
   |
tfsec
   |
Secret scan
   |
Terraform plan
   |
Approval
   |
Apply
```

### Critical security rule

A scanner failure should not automatically be ignored.

Each finding should be:

1.  understood
2.  classified
3.  fixed
4.  documented as accepted risk
5.  or exempted with ownership and justification

# Azure Compute

## Azure Compute

### Virtual Machines

VM engineering should consider:

-   image source
-   OS patching
-   disk encryption
-   identity
-   network placement
-   NSG
-   backup
-   availability
-   monitoring
-   boot diagnostics
-   extensions
-   lifecycle

### VM security baseline

``` text
[ ] No unnecessary public IP
[ ] NSG restricted
[ ] SSH/RDP access controlled
[ ] Managed identity enabled
[ ] Disk encryption configured
[ ] Monitoring enabled
[ ] Backup assessed
[ ] Patching strategy defined
[ ] Least-privilege administration
```

### AKS

For containerized workloads, AKS introduces:

-   cluster identity
-   node pools
-   networking
-   ingress
-   workload identity
-   secrets
-   autoscaling
-   observability
-   policy
-   image security

### Container image pipeline

``` text
Source
  |
Build
  |
Unit Test
  |
Image Scan
  |
SBOM
  |
Registry
  |
Deployment
  |
Runtime Monitoring
```

### Scaling

Scaling decisions should use workload signals such as:

-   CPU
-   memory
-   request rate
-   queue depth
-   latency
-   business transactions

Avoid scaling based on one metric alone when it does not represent user
experience.

# Azure Storage

## Azure Storage

### Storage account design

Important controls include:

-   redundancy
-   TLS
-   encryption
-   public access
-   network rules
-   private endpoints
-   identity
-   lifecycle
-   logging
-   data classification

### Common security baseline

``` text
Public network access       -> minimize
Secure transfer             -> enabled
Minimum TLS                 -> approved baseline
Blob anonymous access       -> disabled unless explicitly required
Network rules               -> restricted
Encryption                  -> enabled
Identity                    -> RBAC / managed identity where supported
Diagnostics                 -> enabled where required
```

### Encryption

Azure Storage provides encryption at rest by default for supported
services.

For workloads requiring customer-controlled keys, design:

``` text
Storage Account
      |
      v
Customer Managed Key
      |
      v
Key Vault
```

### Checkov example

A policy such as `CKV2_AZURE_1` can identify a storage account that does
not meet a customer-managed-key requirement under the applicable Checkov
policy set.

The correct engineering response is to determine whether the data is
classified as requiring CMK and then either:

-   implement the required encryption configuration, or
-   document an approved exception if the control is not applicable.

Do not blindly suppress the finding.

### Data lifecycle

Use lifecycle management for:

-   hot to cool transitions
-   archive
-   retention
-   deletion

Lifecycle rules should reflect business and compliance requirements.

# Azure Database

## Azure Database

Database architecture should address:

-   private connectivity
-   identity
-   encryption
-   backup
-   high availability
-   disaster recovery
-   monitoring
-   maintenance
-   performance
-   cost

### PostgreSQL pattern

A secure pattern can be:

``` text
Application
    |
Private Network
    |
Private Endpoint / Private Access Pattern
    |
Azure Database for PostgreSQL
```

### Database controls

``` text
[ ] Public access evaluated
[ ] Private access evaluated
[ ] Authentication model defined
[ ] TLS enforced
[ ] Backup retention defined
[ ] HA requirement defined
[ ] Monitoring enabled
[ ] Alerting configured
[ ] Data classification documented
[ ] Connection secrets protected
```

### Connection management

Applications should not embed database passwords in source code.

Prefer:

-   managed identity where supported
-   Key Vault
-   secure environment injection
-   short-lived credentials where available

# Azure Monitoring and Observability

## Azure Monitoring and Observability

### Observability pillars

``` text
Metrics + Logs + Traces + Events
```

### Azure Monitor

Azure Monitor provides the platform for collecting and analyzing
telemetry across Azure resources.

### Log Analytics

Log Analytics workspaces centralize logs for query and analysis.

Operational questions should be queryable:

-   What failed?
-   When did it fail?
-   Which resource failed?
-   Which deployment preceded the failure?
-   How many users were affected?
-   Was there a security event?
-   What changed?

### Alert design

Avoid alerting on every metric.

A useful alert should have:

-   clear condition
-   severity
-   owner
-   action
-   runbook
-   expected response time

### Dashboard layers

``` text
Executive
   |
Service
   |
Infrastructure
   |
Security
   |
Cost
```

### SLI / SLO

Define service indicators such as:

-   availability
-   latency
-   error rate
-   throughput

Then define objectives that can drive operational decisions.

### Incident workflow

``` text
Detect
  |
Triage
  |
Contain
  |
Diagnose
  |
Recover
  |
Validate
  |
Document
  |
Prevent recurrence
```

### Post-incident review

Capture:

-   impact
-   timeline
-   detection
-   root cause
-   contributing factors
-   recovery
-   corrective actions
-   preventive actions

# Terraform Engineering

## Terraform Engineering

### Terraform execution model

``` text
Configuration
     |
     v
Provider
     |
     v
Dependency Graph
     |
     v
Refresh / Read
     |
     v
Plan
     |
     v
Apply
```

### Core workflow

``` bash
terraform init
terraform fmt -check
terraform validate
terraform plan
terraform apply
```

### Provider constraints

A provider should have an explicit source and an intentional version
strategy.

Example:

``` hcl
terraform {
  required_providers {
    azurerm = {
      source  = "hashicorp/azurerm"
      version = "4.80.0"
    }
  }
}

provider "azurerm" {
  features {}
}
```

The exact provider version should be chosen according to the repository
compatibility and tested upgrade policy.

### Variables

Variables define the module input contract.

Good variables should have:

-   type
-   description
-   validation where useful
-   sensible defaults only when safe

### Locals

Use locals to simplify repeated expressions and normalize configuration.

### Outputs

Outputs expose stable information from a module.

Examples:

-   resource ID
-   name
-   endpoint
-   subnet ID

Do not expose secrets as outputs unless there is a justified design.

### Data sources

Data sources read existing infrastructure.

Use them when the resource is managed outside the current Terraform
ownership boundary.

### `for_each`

Use `for_each` when resources are keyed by stable logical identifiers.

Example:

``` hcl
resource "azurerm_resource_group" "rg" {
  for_each = var.resource_groups

  name     = each.value.name
  location = each.value.location
}
```

### `count`

Use `count` when a simple numeric or boolean multiplicity is
appropriate.

### `depends_on`

Prefer implicit dependencies through references.

Use explicit `depends_on` only when Terraform cannot infer a real
dependency.

### Lifecycle

Important lifecycle controls include:

-   `prevent_destroy`
-   `create_before_destroy`
-   `ignore_changes`

Each should be used intentionally because lifecycle rules can alter
normal reconciliation behavior.

### Formatting

``` bash
terraform fmt -recursive
```

### Validation

``` bash
terraform validate
```

### Plan

``` bash
terraform plan
```

A plan should be reviewed before production apply.

### Import

Import brings an existing resource under Terraform management.

The process should include:

1.  identify resource
2.  define matching resource block
3.  import resource
4.  plan
5.  reconcile configuration
6.  repeat until the plan matches intent

### Drift

Drift occurs when actual infrastructure changes outside Terraform.

Detection:

``` bash
terraform plan
```

Remediation depends on whether the external change is:

-   intentional and should become code
-   accidental and should be reverted
-   temporary and should be handled explicitly

# Terraform Modules

## Terraform Modules

### Module design

A reusable module should have a small and explicit interface.

Typical structure:

``` text
module/
├── main.tf
├── variables.tf
├── outputs.tf
├── versions.tf
├── README.md
└── examples/
```

### Root module

The root module composes infrastructure.

``` text
Root Module
 |
 +-- Resource Group Module
 |
 +-- Network Module
 |
 +-- Storage Module
 |
 +-- Compute Module
```

### Child module

A child module should avoid environment-specific assumptions.

Bad:

``` text
module internally assumes production names
```

Better:

``` text
caller provides environment-specific values
```

### Module contract

Document:

-   inputs
-   outputs
-   required provider
-   provider versions
-   assumptions
-   examples
-   known limitations

### Module versioning

Use version tags or a controlled registry strategy.

Version changes should communicate compatibility expectations.

### Testing

A mature module can use:

-   `terraform validate`
-   `terraform plan`
-   Checkov
-   tfsec
-   TFLint
-   Terratest

### Module security

A module should avoid:

-   hard-coded secrets
-   unrestricted public access
-   broad IAM/RBAC assignments
-   unbounded CIDRs
-   weak defaults

### Module review checklist

``` text
[ ] Inputs typed
[ ] Inputs documented
[ ] Outputs documented
[ ] Provider source defined
[ ] Version constraint defined
[ ] Naming standardized
[ ] Tags supported
[ ] Security baseline implemented
[ ] Tests available
[ ] README available
[ ] Example available

# Terraform State

## Terraform State

### Why state exists

Terraform state maps configuration resources to real infrastructure objects.

Conceptually:

```text
Terraform Configuration
        |
        v
Terraform State
        |
        v
Azure Resource IDs
```

### Remote state

For Azure, an Azure Storage backend can provide centralized state
storage.

A typical backend uses:

-   storage account
-   blob container
-   state key

### State security

Protect state because it can contain sensitive infrastructure
information and, depending on configuration, sensitive values.

Controls:

-   restricted access
-   encryption
-   network controls
-   RBAC
-   state locking
-   backups / recovery

### State locking

Locking prevents concurrent operations from modifying the same state
simultaneously.

### State key strategy

Use separate keys for separate state boundaries.

Example:

``` text
tfstate/
  platform.tfstate
  network-prod.tfstate
  app-prod.tfstate
```

### Backend initialization

Example conceptual command:

``` bash
terraform init
```

Backend configuration should be supplied securely through pipeline
configuration rather than committed secrets.

### State anti-patterns

Avoid:

-   committing `.tfstate`
-   sharing local state
-   manually editing state without a controlled procedure
-   using one state for unrelated environments
-   exposing backend credentials

### `.gitignore`

A Terraform repository should normally ignore:

``` gitignore
.terraform/
*.tfstate
*.tfstate.*
*.tfvars
crash.log
.terraformrc
terraform.rc
override.tf
override.tf.json
*_override.tf
*_override.tf.json
```

A repository may intentionally commit example variable files that
contain no secrets.

# Terraform Security

## Terraform Security

### Security scanning layer

Use multiple controls because each tool catches different classes of
issues.

``` text
Terraform Code
     |
     +--> Terraform Validate
     |
     +--> TFLint
     |
     +--> Checkov
     |
     +--> tfsec
     |
     +--> Secret Scan
     |
     +--> Plan Review
```

### Checkov

Checkov scans infrastructure as code against security and compliance
policies.

Example:

``` bash
checkov -d .
```

A failed check should be treated as a signal for engineering review.

### tfsec

tfsec evaluates Terraform configuration for security issues.

### TFLint

TFLint focuses on Terraform linting and provider-aware validation.

### TruffleHog

TruffleHog helps detect exposed secrets and credentials.

### Trivy

Trivy can be used for broader security scanning, including container and
repository-oriented use cases depending on the integration.

### Terratest

Terratest provides infrastructure testing using Go.

A typical test can:

1.  deploy test infrastructure
2.  validate outputs
3.  run assertions
4.  destroy resources

### Security exception process

Never convert a failing scan into a permanent ignored result without
justification.

Record:

-   check ID
-   resource
-   reason
-   risk
-   owner
-   expiration/review date
-   compensating control

# Terraform CI/CD

## Terraform CI/CD

### Recommended pipeline stages

``` text
Checkout
  |
Format
  |
Validate
  |
Lint
  |
Security Scan
  |
Secret Scan
  |
Cost Estimate
  |
Init
  |
Plan
  |
Approval
  |
Apply
```

### Why `checkout` matters

The pipeline needs the repository content before Terraform can operate.

A clean checkout can prevent stale workspace files from affecting a
build, but it should be used intentionally according to the
agent/workspace strategy.

### Init

`terraform init`:

-   initializes the working directory
-   installs providers
-   configures backend
-   prepares modules

### Validate

`terraform validate` checks configuration syntax and internal
consistency.

### Plan

`terraform plan` calculates proposed changes.

### Apply

`terraform apply` executes approved changes.

### Plan artifact

For controlled deployments, save the reviewed plan:

``` bash
terraform plan -out=tfplan
```

Then apply the saved plan when the delivery design supports that
workflow.

### Manual approval

Production apply should have an explicit approval boundary when
organizational policy requires it.

### Environment separation

A mature pipeline separates:

-   development
-   test
-   staging
-   production

### Failure behavior

Fail fast for:

-   syntax errors
-   authentication failures
-   security violations
-   invalid Terraform configuration
-   unavailable dependencies

Do not hide failures with `continueOnError` unless there is a deliberate
non-blocking quality gate.

### Service connections

Azure DevOps service connections provide pipeline authentication to
Azure resources.

Prefer:

-   least privilege
-   scoped permissions
-   federation where supported
-   controlled ownership
-   auditable access

# Azure DevOps

## Azure DevOps

### Pipeline structure

A production YAML pipeline commonly separates:

-   stages
-   jobs
-   steps
-   tasks
-   environments

### Example stage model

``` yaml
stages:
- stage: Validate
- stage: Security
- stage: Plan
- stage: Approval
- stage: Apply
```

### Azure service connection

The service connection is the pipeline's Azure authentication boundary.

Use it to avoid embedding user credentials in scripts.

### Variables

Use pipeline variables for non-secret configuration.

Use secret variables or supported secret stores for sensitive data.

### Secure files and Key Vault

For sensitive material, prefer controlled secret management rather than
plaintext YAML.

### Self-hosted agent

A self-hosted agent can be useful when:

-   private network access is required
-   custom tools are installed
-   enterprise network controls apply
-   build dependencies are specialized

The agent should be treated as production infrastructure.

### Agent hardening

-   keep OS patched
-   restrict local administrator access
-   protect credentials
-   monitor processes
-   rotate registration credentials
-   minimize installed software
-   isolate workloads when appropriate

### Pipeline troubleshooting

When a task fails:

1.  read the first error
2.  identify the executing command
3.  inspect the working directory
4.  validate tool path
5.  validate environment variables
6.  validate service connection
7.  reproduce locally
8.  compare local and agent environments

# GitHub Actions

## GitHub Actions

### Workflow model

``` text
Event
  |
Workflow
  |
Job
  |
Runner
  |
Step
```

### Security

Prefer OIDC/workload identity federation over long-lived cloud secrets
where supported.

### Typical Terraform workflow

``` yaml
name: Terraform

on:
  pull_request:
  push:
    branches:
      - main

jobs:
  terraform:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4

      - name: Terraform Init
        run: terraform init

      - name: Terraform Validate
        run: terraform validate

      - name: Terraform Plan
        run: terraform plan
```

The exact authentication and backend configuration should be adapted to
the organization's Azure identity model.

### Branch protection

Protect production branches with:

-   pull requests
-   required reviews
-   status checks
-   security gates
-   restricted direct pushes

### Reusable workflows

Reusable workflows help standardize:

-   Terraform validation
-   security scanning
-   container scanning
-   release processes

# DevSecOps

## DevSecOps

### Shift-left model

``` text
Developer
   |
IDE / Pre-commit
   |
Pull Request
   |
Static Analysis
   |
IaC Security
   |
Secret Detection
   |
Dependency / Container Scan
   |
Plan
   |
Approval
   |
Deployment
   |
Runtime Security
```

### Security gates

  Gate                 Purpose
  -------------------- ----------------------------------------
  Terraform validate   Configuration correctness
  TFLint               Terraform linting
  Checkov              IaC policy checks
  tfsec                IaC security checks
  TruffleHog           Secret detection
  Trivy                Vulnerability scanning
  Terratest            Infrastructure behavior
  SonarQube            Code quality/security where applicable

### Blocking policy

Not every warning must block every pipeline.

Define severity policy:

``` text
Critical -> Block
High     -> Block
Medium   -> Review / policy dependent
Low      -> Track
Informational -> Observe
```

The exact thresholds should be determined by organizational risk policy.

### DevSecOps metrics

Useful metrics include:

-   security findings per build
-   mean time to remediate
-   percentage of builds passing security gates
-   secrets prevented from merge
-   infrastructure policy compliance
-   vulnerability aging
-   deployment frequency
-   change failure rate

### Golden path

A platform team can provide a secure default pipeline so teams do not
have to design DevSecOps controls from scratch.

# Policy as Code

## Policy as Code

Policy as Code turns governance rules into version-controlled, testable
definitions.

### Benefits

-   repeatability
-   reviewability
-   auditability
-   automation
-   consistency

### Example policy lifecycle

``` text
Policy Requirement
       |
       v
Policy Definition
       |
       v
Test
       |
       v
Pull Request
       |
       v
Approval
       |
       v
Pipeline
       |
       v
Enforcement
       |
       v
Monitoring
```

### Policy categories

-   region restrictions
-   SKU restrictions
-   public network access
-   encryption
-   diagnostic settings
-   identity requirements
-   tagging
-   private connectivity

### Terraform policy controls

Terraform security scanners provide an early feedback loop before
resources reach Azure.

### Azure Policy controls

Azure Policy provides resource-level governance after configuration
reaches the Azure control plane.

### Combined model

``` text
Developer Time
   |
Terraform Security Scan
   |
CI/CD
   |
Azure Policy
   |
Runtime Monitoring
```

The same security intent should ideally be represented consistently
across these layers.

# Secret Management

## Secret Management

### Secret hierarchy

Prefer this order:

``` text
Workload Identity
       >
Managed Identity
       >
Federated Identity
       >
Short-lived credential
       >
Long-lived secret
```

The exact choice depends on service support.

### Never commit

-   passwords
-   client secrets
-   private keys
-   tokens
-   storage account keys
-   database credentials
-   API keys

### `.gitignore` is not a security boundary

Ignoring a file prevents it from being tracked in normal Git operations,
but it does not remove a secret that was already committed.

If a secret is exposed:

1.  revoke or rotate it
2.  investigate access
3.  remove it from repository history as required
4.  update consumers
5.  add prevention controls

### Key Vault integration

A common pattern:

``` text
Pipeline / Workload Identity
          |
          v
Microsoft Entra ID
          |
          v
Azure Key Vault
          |
          v
Secret / Key / Certificate
```

### Secret scanning workflow

``` text
Pre-commit
    |
Pull Request
    |
CI Secret Scan
    |
Repository Security
    |
Credential Rotation
```

# Container and Kubernetes Security

## Container and Kubernetes Security

### Image lifecycle

``` text
Dockerfile
   |
Build
   |
Lint
   |
Vulnerability Scan
   |
SBOM
   |
Sign / Verify
   |
Registry
   |
Deploy
```

### AKS security considerations

-   Entra integration
-   workload identity
-   network policies
-   private cluster where required
-   node pool isolation
-   image provenance
-   registry access
-   secret handling
-   pod security
-   logging
-   monitoring

### Runtime identity

Avoid storing Azure service credentials inside container images.

Use workload identity patterns where supported.

### Kubernetes network design

Separate:

-   ingress
-   application
-   data
-   management

Use explicit policies rather than assuming that network reachability
equals authorization.

### Container scan policy

A release policy can block:

-   critical vulnerabilities
-   known exploitable high vulnerabilities
-   unsigned images
-   prohibited base images
-   exposed secrets

The exact thresholds should match organizational risk.

# Networking Security Patterns

## Networking Security Patterns

### Internet-facing workload

``` text
Internet
   |
   v
DDoS Protection
   |
   v
Application Gateway / WAF
   |
   v
Application subnet
   |
   v
Private data services
```

### Private workload

``` text
Corporate Network
      |
VPN / ExpressRoute / WAN
      |
Hub
      |
Firewall
      |
Spoke
      |
Private Endpoint
      |
PaaS Service
```

### Egress control

Centralized egress can provide:

-   inspection
-   logging
-   destination restrictions
-   threat intelligence
-   cost visibility

### DNS

DNS is foundational for private connectivity.

A private endpoint design should explicitly document:

-   private DNS zones
-   VNet links
-   DNS forwarding
-   resolver path
-   split-horizon requirements

### Network troubleshooting checklist

``` text
[ ] DNS resolves
[ ] Route exists
[ ] NSG permits
[ ] Firewall permits
[ ] Peering is healthy
[ ] Private DNS is linked
[ ] Endpoint is approved
[ ] Service is healthy
[ ] Application listener is active
```

# FinOps and Cost Optimization

## FinOps and Cost Optimization

### Cost is an architecture attribute

Cost should be evaluated before deployment, not only after the invoice
arrives.

### Infracost

Infracost can estimate Terraform-related infrastructure costs before
deployment.

Conceptual workflow:

``` text
Terraform
   |
Infracost
   |
Cost Diff
   |
Pull Request
   |
Approval
```

### Cost review

Review:

-   compute sizing
-   storage redundancy
-   network egress
-   database tier
-   idle resources
-   public IPs
-   log retention
-   monitoring volume
-   backup retention
-   environment lifetime

### OpenCost

OpenCost can support cost visibility in Kubernetes environments.

### Rightsizing

Rightsizing should use actual utilization.

Do not downsize production resources solely because an invoice looks
high.

### Cost governance

Use:

-   budgets
-   alerts
-   tags
-   resource ownership
-   scheduled shutdowns for non-production
-   SKU policy
-   cost allocation

### Cost optimization checklist

``` text
[ ] Resource owner exists
[ ] Cost center exists
[ ] Environment tagged
[ ] Idle resources reviewed
[ ] VM sizing reviewed
[ ] Storage tier reviewed
[ ] Log retention reviewed
[ ] Backup retention reviewed
[ ] Egress reviewed
[ ] Non-prod schedules considered
[ ] Monthly cost estimate reviewed
```

# Reliability and Disaster Recovery

## Reliability and Disaster Recovery

### Reliability layers

``` text
Application
   |
Compute
   |
Network
   |
Data
   |
Region
```

Each layer needs an explicit failure strategy.

### RTO and RPO

**RTO** defines how quickly service should be restored.

**RPO** defines how much data loss is acceptable.

### DR design

A DR strategy should document:

-   primary region
-   secondary region
-   replication
-   backup
-   failover mechanism
-   DNS
-   dependencies
-   runbook
-   ownership
-   test frequency

### Backup

Backups are useful only when restore has been tested.

### DR test

``` text
Plan
  |
Simulate
  |
Failover
  |
Validate
  |
Failback
  |
Measure
  |
Improve
```

### Availability

Use appropriate Azure capabilities such as:

-   availability zones
-   load balancing
-   redundant instances
-   managed database HA
-   multi-region patterns where required

Avoid adding redundancy without understanding the workload's real
failure modes.

# Platform Engineering

## Platform Engineering

Platform Engineering creates reusable internal capabilities so
application teams can consume infrastructure safely without rebuilding
platform controls every time.

### Platform product

Treat the platform as a product.

Users:

-   application developers
-   engineering teams
-   security teams
-   operations teams

### Golden path

A golden path should provide:

``` text
Repository
   |
Pipeline
   |
Identity
   |
Infrastructure
   |
Security
   |
Observability
   |
Cost
```

### Terraform module catalog

Possible platform modules:

-   resource group
-   VNet
-   subnet
-   NSG
-   private endpoint
-   Key Vault
-   storage account
-   VM
-   AKS
-   monitoring
-   diagnostics

### Platform standards

Every module should have:

-   documentation
-   examples
-   versioning
-   security defaults
-   ownership
-   support model

### Self-service

Self-service should not mean unrestricted access.

The platform should provide controlled choices:

``` text
Developer Request
       |
Approved Template
       |
Validated Inputs
       |
Policy Checks
       |
Automated Provisioning
```

# GenAI for Cloud Engineering

## GenAI for Cloud Engineering

GenAI can accelerate cloud engineering when it is used as an assistant
rather than an uncontrolled deployment authority.

### High-value use cases

-   Terraform explanation
-   Terraform review
-   YAML troubleshooting
-   log summarization
-   incident triage
-   documentation generation
-   runbook drafting
-   architecture comparison
-   security finding explanation
-   cost anomaly investigation
-   migration planning

### AI-assisted IaC review

``` text
Terraform PR
    |
Static Checks
    |
Security Scans
    |
GenAI Review
    |
Human Review
    |
Approval
```

### Guardrails

GenAI should not independently:

-   grant production Owner access
-   rotate credentials without controls
-   destroy production infrastructure
-   bypass security gates
-   approve its own changes

### Human-in-the-loop

For high-impact operations:

``` text
AI Suggestion
     |
Evidence
     |
Engineer Review
     |
Approval
     |
Execution
```

### GenAI security

Never send confidential infrastructure data, credentials or sensitive
customer information to an AI system unless the organization's approved
data handling model explicitly permits it.

### Documentation automation

AI can help transform:

-   Terraform modules
-   architecture decisions
-   pipeline definitions
-   incident notes

into structured engineering documentation.

# Enterprise Delivery Workflow

## Enterprise Delivery Workflow

### End-to-end workflow

``` text
Requirement
   |
Architecture
   |
Threat Model
   |
Terraform Module Design
   |
Pull Request
   |
Format
   |
Validate
   |
Lint
   |
Security
   |
Secret Scan
   |
Cost
   |
Plan
   |
Approval
   |
Apply
   |
Monitor
   |
Audit
   |
Optimize
```

### Architecture review

Before implementation, confirm:

-   business requirement
-   availability
-   security
-   network
-   identity
-   data
-   compliance
-   cost
-   observability
-   DR

### Threat modeling

Ask:

-   What can be exposed?
-   What identity can be compromised?
-   What data is sensitive?
-   What happens if the network is breached?
-   What is the blast radius?
-   How is the event detected?
-   How is recovery performed?

### Change management

Every production change should have:

-   scope
-   risk
-   validation
-   rollback
-   owner
-   approval
-   evidence

### Rollback

Rollback must be technically possible and operationally documented.

For infrastructure, rollback may mean:

-   reverting Terraform code
-   applying a previous known-good plan
-   restoring data
-   reverting configuration
-   switching traffic
-   failing over

# Project Portfolio

## Project Portfolio

### 🏗️ Enterprise Azure Landing Zone

A reusable landing-zone architecture focused on:

-   management groups
-   multi-subscription governance
-   policy
-   RBAC
-   hub-and-spoke connectivity
-   shared services
-   workload isolation

### 📦 Terraform Module Framework

Reusable Azure infrastructure modules covering patterns such as:

-   Resource Groups
-   VNets
-   subnets
-   NSGs
-   network interfaces
-   virtual machines
-   storage accounts
-   Azure Bastion

The module approach standardizes provisioning and reduces duplicated
infrastructure code.

### 🛡️ Azure DevSecOps Pipeline

A security-first infrastructure pipeline combining:

-   Azure DevOps
-   Terraform
-   TFLint
-   tfsec
-   Checkov
-   TruffleHog
-   Terratest
-   cost estimation
-   plan review
-   controlled apply

### 🌐 Azure Hub-Spoke Networking

A scalable network architecture based on:

-   hub VNet
-   spoke VNets
-   peering
-   Azure Firewall
-   NSGs
-   private endpoints
-   Bastion
-   controlled routing

### 📊 Azure Monitoring and Observability

Centralized operational visibility using:

-   Azure Monitor
-   Log Analytics
-   Grafana
-   Nagios
-   Zabbix
-   OpenCost

### 🔐 Azure Security and Governance

Security patterns covering:

-   RBAC
-   PIM
-   managed identities
-   Key Vault
-   Azure Policy
-   Defender for Cloud
-   Zero Trust

### 🤖 Infrastructure Automation

Automation concepts for:

-   drift detection
-   remediation
-   documentation
-   repetitive operations
-   GenAI-assisted engineering workflows

# Operational Runbooks

## Operational Runbooks

### Terraform pipeline failure

``` text
1. Read the first failing task.
2. Identify the command executed.
3. Verify working directory.
4. Verify repository checkout.
5. Verify tool availability.
6. Verify authentication.
7. Verify backend.
8. Verify provider version.
9. Reproduce locally.
10. Correct the smallest root cause.
```

### Terraform init failure

Check:

-   backend configuration
-   service connection
-   subscription
-   resource group
-   storage account
-   container
-   state key
-   permissions
-   network access

### Terraform validate failure

Check:

-   syntax
-   variable declarations
-   provider blocks
-   resource arguments
-   module references
-   type mismatches

### Terraform plan failure

Check:

-   credentials
-   subscription
-   resource existence
-   state
-   provider compatibility
-   data sources
-   API permissions
-   SKU availability

### Checkov failure

Do not immediately suppress.

``` text
Finding
  |
Understand
  |
Applicable?
  |
+----+----+
|         |
Yes       No
|         |
Fix       Document
|         |
Pass      Approved exception
```

### Infracost failure

Common prerequisites include:

-   executable available
-   valid command syntax
-   Terraform path exists
-   authentication/API configuration available when required
-   provider/resource support
-   network access if the tool requires external services

### Azure authentication failure

Check:

``` text
Identity
   |
Service Connection
   |
Subscription
   |
RBAC
   |
Resource Scope
```

### Network failure

Check in order:

``` text
DNS -> Route -> NSG -> Firewall -> Peering -> Endpoint -> Application
```

### Production incident

``` text
Detect
Triage
Contain
Communicate
Recover
Validate
Document
Prevent
```

# Security Checklists

## Security Checklists

### Terraform repository

``` text
[ ] No state files committed
[ ] No secrets committed
[ ] Provider source pinned
[ ] Provider upgrade process defined
[ ] Modules documented
[ ] Security scanning enabled
[ ] Secret scanning enabled
[ ] Pull requests protected
[ ] Production apply controlled
[ ] Backend secured
```

### Azure landing zone

``` text
[ ] Management groups
[ ] Subscriptions
[ ] Policy
[ ] RBAC
[ ] PIM
[ ] Connectivity
[ ] DNS
[ ] Firewall
[ ] Logging
[ ] Defender
[ ] Backup
[ ] Cost governance
```

### Storage

``` text
[ ] TLS
[ ] Encryption
[ ] Network restriction
[ ] Public access reviewed
[ ] Identity access
[ ] Diagnostic logging
[ ] Lifecycle
[ ] Backup/recovery
[ ] CMK requirement assessed
```

### CI/CD

``` text
[ ] Branch protection
[ ] Pull request
[ ] Validate
[ ] Lint
[ ] Security scan
[ ] Secret scan
[ ] Cost estimate
[ ] Plan
[ ] Approval
[ ] Apply
[ ] Audit
```

### Production readiness

``` text
[ ] Owner
[ ] Monitoring
[ ] Alerting
[ ] Backup
[ ] DR
[ ] RTO
[ ] RPO
[ ] Runbook
[ ] Security review
[ ] Cost review
[ ] Rollback plan

# Terraform Command Reference

## Terraform Command Reference

### Initialize

```bash
terraform init
```

### Format

``` bash
terraform fmt
terraform fmt -check
terraform fmt -recursive
```

### Validate

``` bash
terraform validate
```

### Plan

``` bash
terraform plan
```

### Save plan

``` bash
terraform plan -out=tfplan
```

### Apply

``` bash
terraform apply
terraform apply tfplan
```

### Destroy

``` bash
terraform destroy
```

Use destroy only when the scope and consequences are explicitly
understood.

### Show state

``` bash
terraform show
```

### List state

``` bash
terraform state list
```

### Import

``` bash
terraform import <resource_address> <resource_id>
```

### Providers

``` bash
terraform providers
```

### Graph

``` bash
terraform graph
```

### Output

``` bash
terraform output
```

### Refresh-oriented planning

Use current Terraform workflows rather than treating `terraform refresh`
as a universal operational command; understand the implications for
state before using state-changing operations.

# Azure CLI Reference

## Azure CLI Reference

### Login

``` bash
az login
```

### Subscription

``` bash
az account show
az account list
az account set --subscription "<subscription-id>"
```

### Resource group

``` bash
az group create   --name rg-example   --location centralindia
```

### List resource groups

``` bash
az group list -o table
```

### Resource list

``` bash
az resource list -o table
```

### Storage account list

``` bash
az storage account list -o table
```

### VNet list

``` bash
az network vnet list -o table
```

### NSG list

``` bash
az network nsg list -o table
```

### Private endpoints

``` bash
az network private-endpoint list -o table
```

### Role assignment

``` bash
az role assignment list --assignee <object-id>
```

### Policy

``` bash
az policy assignment list -o table
```

### Monitor

``` bash
az monitor activity-log list
```

# Git Reference

## Git Reference

### Clone

``` bash
git clone <repository-url>
```

### Status

``` bash
git status
```

### Branch

``` bash
git branch
```

### Create branch

``` bash
git checkout -b feature/terraform-security
```

### Stage

``` bash
git add .
```

### Commit

``` bash
git commit -m "Add Terraform security checks"
```

### Push

``` bash
git push origin feature/terraform-security
```

### Pull

``` bash
git pull
```

### View history

``` bash
git log --oneline --decorate --graph
```

### Review changes

``` bash
git diff
git diff --staged
```

### Restore working tree changes

``` bash
git restore <file>
```

Use destructive Git commands carefully, especially when rewriting shared
history.

### Repository hygiene

Never commit:

``` text
.terraform/
*.tfstate
*.tfstate.*
secrets
private keys
local credentials
temporary plan files
```

# PowerShell Reference

## PowerShell Reference

### Check executable

``` powershell
Test-Path "C:\Tools\terraform.exe"
```

### Execute executable

``` powershell
& "C:\Tools\terraform.exe" version
```

### Capture exit code

``` powershell
& "C:\Tools\checkov.exe" -d "."
if ($LASTEXITCODE -ne 0) {
    exit 1
}
```

### Set location

``` powershell
Set-Location "C:\path\to\terraform"
```

### Environment variable

``` powershell
$env:INFRACOST_API_KEY
```

### Test path

``` powershell
if (!(Test-Path $path)) {
    Write-Error "Path not found"
    exit 1
}
```

### Pipeline principle

A PowerShell script embedded in an Azure DevOps `PowerShell@2` task must
contain PowerShell only inside the `script: |` block.

Do not paste YAML task definitions inside the PowerShell script body.

Correct structure:

``` yaml
- task: PowerShell@2
  inputs:
    targetType: inline
    script: |
      Write-Host "Running security scan"
      & "C:\Tools\checkov.exe" -d "."
```

### Tool paths

Keep executable paths explicit when using a controlled self-hosted
agent, and validate the path before execution.

# Bash Reference

## Bash Reference

### Variables

``` bash
TERRAFORM_DIR="./environments/parent_module"
```

### Path check

``` bash
test -d "$TERRAFORM_DIR"
```

### Execute

``` bash
terraform -chdir="$TERRAFORM_DIR" validate
```

### Exit handling

``` bash
terraform plan
status=$?

if [ "$status" -ne 0 ]; then
  echo "Terraform plan failed"
  exit "$status"
fi
```

### Pipeline principle

Keep shell scripts small, deterministic and explicit about exit codes.

Avoid hiding command failures with unconditional success handling.

# Interview-Level Architecture Questions

## Interview-Level Architecture Questions

### Azure Landing Zone

**Question:** What is an Azure Landing Zone?

**Answer:** It is a standardized Azure platform foundation that provides
identity, governance, networking, security and operational guardrails so
workload teams can deploy consistently.

### Hub and Spoke

**Question:** Why use hub and spoke?

**Answer:** It centralizes shared network services while isolating
workload networks into spokes. This can improve governance, segmentation
and operational consistency.

### Terraform state

**Question:** Why use remote state?

**Answer:** Remote state centralizes Terraform's state, supports
collaboration and enables controlled locking and access management.

### `for_each` versus `count`

**Question:** When do you prefer `for_each`?

**Answer:** When resources are naturally identified by stable keys. This
avoids index-oriented identity and makes individual instances easier to
manage.

### Data source

**Question:** When should a data source be used?

**Answer:** When Terraform needs to read an existing object that is
outside the current resource ownership boundary.

### Service connection

**Question:** Why use an Azure DevOps service connection?

**Answer:** It provides a controlled authentication boundary for
pipeline-to-Azure operations without embedding interactive user
credentials in pipeline scripts.

### Checkov

**Question:** What does Checkov do?

**Answer:** It scans infrastructure as code against security and
compliance policies and reports violations before infrastructure is
deployed.

### Infracost

**Question:** Where does Infracost fit?

**Answer:** It provides cost estimation and cost-diff feedback from
infrastructure definitions, making cloud cost visible during engineering
review.

### Private endpoint

**Question:** Why use a private endpoint?

**Answer:** It provides private network access to supported Azure
services through a private IP in a VNet, reducing dependence on public
network exposure.

### Managed identity

**Question:** Why prefer managed identity?

**Answer:** It avoids storing long-lived credentials in application or
pipeline configuration and allows Azure-managed identity authentication
for supported services.

### PIM

**Question:** What problem does PIM solve?

**Answer:** It reduces standing privileged access by making privileged
roles eligible and activated for controlled periods.

### Terraform pipeline

**Question:** What should happen before apply?

**Answer:** Validate, lint, security scan, secret scan, cost review and
plan should complete according to policy, followed by the required
approval boundary.

# Current Focus

## Current Focus

### Enterprise Azure Architecture

-   Landing Zone design
-   governance
-   network architecture
-   identity
-   security
-   observability
-   cost

### DevSecOps

-   secure Terraform pipelines
-   policy-as-code
-   IaC security
-   secret scanning
-   controlled releases

### Platform Engineering

-   reusable Terraform modules
-   golden paths
-   self-service infrastructure
-   standardized CI/CD

### GenAI

-   infrastructure review
-   documentation
-   incident analysis
-   automation assistance
-   secure engineering workflows

# Certifications

## Certifications

::: {align="center"}
![AZ-104](https://img.shields.io/badge/AZ--104-Azure_Administrator_Associate-0078D4?style=for-the-badge&logo=microsoftazure&logoColor=white)
![AZ-305](https://img.shields.io/badge/AZ--305-Azure_Solutions_Architect_Expert-8A2BE2?style=for-the-badge&logo=microsoftazure&logoColor=white)
:::

### AZ-104

Microsoft Certified: Azure Administrator Associate.

Relevant capability areas include:

-   Azure identity
-   governance
-   storage
-   compute
-   networking
-   monitoring

### AZ-305

Microsoft Certified: Azure Solutions Architect Expert.

Relevant architecture areas include:

-   identity
-   governance
-   data
-   networking
-   compute
-   resilience
-   security

# Engineering Principles

## Engineering Principles

### Principle 01 --- Automate the repeatable

If a task is performed frequently, identify whether it can become code,
a module, a pipeline or a runbook.

### Principle 02 --- Secure the default

The easiest path should also be the safest practical path.

### Principle 03 --- Minimize blast radius

Separate:

-   subscriptions
-   networks
-   identities
-   permissions
-   state
-   workloads

when the risk model requires isolation.

### Principle 04 --- Prefer explicit ownership

Every important resource should have an owner and a business context.

### Principle 05 --- Review before mutation

Production infrastructure should not be changed blindly.

### Principle 06 --- Observe before optimizing

Use real telemetry before rightsizing compute, changing retention or
altering architecture.

### Principle 07 --- Treat policy as code

Governance should be versioned, reviewed and tested where practical.

### Principle 08 --- Make recovery a feature

Backup and DR are part of architecture, not documentation after
deployment.

### Principle 09 --- Design for operators

A platform that developers can deploy but operators cannot troubleshoot
is incomplete.

### Principle 10 --- Human approval for high-impact AI actions

AI can accelerate analysis, but production mutation remains governed by
engineering controls.

------------------------------------------------------------------------

## Professional Engineering Scorecard

  Area             Target state
  ---------------- -------------------------------------
  Infrastructure   Declarative and repeatable
  Security         Shift-left and continuous
  Identity         Least privilege
  Network          Segmented and observable
  State            Remote and protected
  Delivery         Automated with approval boundaries
  Governance       Policy-driven
  Monitoring       Metrics + logs + alerts
  Cost             Visible before and after deployment
  DR               Tested
  Modules          Versioned and reusable
  Documentation    Maintained with code
  AI               Assisted, governed and auditable

------------------------------------------------------------------------

## Closing Statement

The goal is not simply to provision Azure resources.

The goal is to build a platform in which:

``` text
Architecture is intentional
Infrastructure is reproducible
Security is automated
Identity is least-privileged
Networking is segmented
Delivery is controlled
Cost is visible
Operations are observable
Recovery is tested
Automation is scalable
AI is governed
```

**Microsoft Azure · Terraform · DevSecOps · Cloud Security · Platform
Engineering · GenAI**

`<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0A0E27,40:0078D4,100:8A2BE2&height=180&section=footer&animation=fadeIn" width="100%"/>`{=html}

::: {align="center"}
**⭐ Build it as code. Secure it by default. Operate it with evidence.**
:::

## Terraform Variable Design

-   Use typed variables to make module contracts explicit.
-   Use validation rules for values with known constraints.
-   Keep secrets out of default values and source control.
-   Use objects for structured configuration instead of parallel
    variables.
-   Use maps when stable keys identify multiple instances.
-   Use sets when uniqueness is the primary requirement.
-   Use optional object attributes only when the module can safely
    define defaults.
-   Document whether a variable is environment-specific or
    platform-standard.
-   Keep module input names aligned with their actual semantics.
-   Do not create a variable simply to avoid writing a local expression.

## Terraform Dependency Graph

-   Terraform builds a dependency graph from resource references.
-   References create implicit dependencies and are preferred.
-   Explicit depends_on should be reserved for dependencies Terraform
    cannot infer.
-   Overusing depends_on can reduce plan parallelism and obscure
    architecture.
-   Module boundaries should expose meaningful dependencies through
    inputs and outputs.
-   Data sources can introduce dependencies when their inputs reference
    managed resources.
-   Dependency cycles indicate a design problem and should be resolved
    structurally.

## Terraform Provider Strategy

-   Declare provider source addresses explicitly.
-   Keep provider version constraints deliberate.
-   Review provider release notes before major upgrades.
-   Run validation, plan and security tests after upgrades.
-   Use provider aliases when multiple Azure contexts are genuinely
    required.
-   Do not copy provider blocks into child modules without a clear
    reason.
-   Keep authentication outside reusable module logic.

## Azure Network Design Review

-   Confirm address spaces before creating peering relationships.
-   Reserve address space for future platform expansion.
-   Separate workload tiers where the threat model requires it.
-   Use NSGs for subnet or NIC traffic controls as appropriate.
-   Use route tables when traffic inspection or custom routing is
    required.
-   Document firewall paths to avoid asymmetric routing.
-   Design DNS before private endpoints.
-   Test name resolution from the actual workload subnet.

## Azure Identity Review

-   Map every workload to an identity.
-   Remove unused service principals.
-   Prefer managed identity for Azure-hosted workloads where supported.
-   Use RBAC scopes that match the resource ownership boundary.
-   Review Owner and User Access Administrator assignments regularly.
-   Use PIM for eligible privileged roles where appropriate.
-   Require MFA for privileged human access.
-   Audit service connection permissions.

## Pipeline Quality Gates

-   Formatting is a low-cost first gate.
-   Validation confirms Terraform configuration consistency.
-   Linting catches style and provider-aware issues.
-   IaC scanning catches known insecure patterns.
-   Secret scanning catches accidental credential exposure.
-   Cost estimation exposes architectural cost before deployment.
-   Plan provides the mutation preview.
-   Approval establishes human governance before production mutation.
-   Apply should use the same intended code and controlled state.

## Incident Response

-   Define severity before an incident occurs.
-   Identify the incident commander and technical owner.
-   Preserve useful evidence during investigation.
-   Separate containment from permanent remediation.
-   Communicate impact using facts rather than speculation.
-   Record the timeline using timestamps.
-   Validate recovery from the user perspective.
-   Create preventive actions with owners and due dates.
-   Feed lessons learned back into platform automation.

## Production Readiness Matrix

  Control      Evidence
  ------------ ------------------------------------------
  Identity     RBAC assignments and access review
  Network      Approved topology and connectivity tests
  Security     Scanner results and exceptions
  Terraform    Versioned code and reviewed plan
  State        Protected remote backend
  Monitoring   Dashboards and actionable alerts
  Backup       Restore test evidence
  DR           Failover test evidence
  Cost         Forecast and budget ownership
  Operations   Runbook and on-call ownership

## Architecture Decision Records

An ADR should capture the context, decision, alternatives and
consequences. Record why a design was chosen, not only what was
deployed. Include rejected alternatives when they materially influenced
the decision. Link the ADR to implementation code when possible. Review
ADRs when assumptions materially change.

## Change Risk Model

Low-risk changes can follow an automated path. Medium-risk changes may
require additional review or testing. High-risk production changes
should have explicit approval and rollback evidence. Security-impacting
changes should include security review when required. Network boundary
changes should be treated as potentially high impact. Identity
permission changes should be reviewed for blast radius. State/backend
changes require special care because they affect Terraform control.
