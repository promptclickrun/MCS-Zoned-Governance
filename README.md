# Copilot Studio Agent Governance  
## Zoned Governance Framework: Determining Your Agent’s Zone  
*March 2026*

The Copilot Studio Zoned Governance Framework provides a structured approach to classifying agents based on their scope, audience, data access, and complexity. By assigning each agent to a governance zone—**Green, Yellow, or Red**—organizations can ensure the right level of oversight is applied without introducing unnecessary friction for low-risk innovation. This framework empowers citizen developers to build confidently while giving IT teams clear guardrails for higher-stakes, enterprise-wide deployments.

---

## Zone Overview — Visual Summary

| Zone               | Track             | Who Builds         | Audience              | Admin Posture    |
|--------------------|-------------------|--------------------|-----------------------|------------------|
| **Zone 1 — Green**  | Safe Innovation   | Citizen Dev        | Personal / Workgroup  | Hands-off Admin  |
| **Zone 2 — Yellow** | Guided Development| Maker + IT Guidance| Department            | Active Oversight |
| **Zone 3 — Red**    | IT Managed        | Pro-Dev / IT-Approved | Enterprise-Wide     | Full IT Control  |

---

## Green Zone — Safe Innovation Zone

The Green Zone is designed for low-risk, personal or small-workgroup agents built by citizen developers. Agents in this zone operate within Microsoft 365 native data sources and are deployed in personal developer environments, requiring no special administrative oversight. Administrators can safely adopt a hands-off posture, confident that platform defaults and DLP policies provide adequate governance.

### An agent lands in the **GREEN ZONE** when:  
- Built in a personal Developer environment  
- Grounded in M365 data only (SharePoint, OneDrive, Teams)  
- Shared with a small personal workgroup only  
- No external connectors or actions required  
- Maker fully owns the management lifecycle  
- Low complexity — no autonomous actions or multi-agent orchestration  
- Admins can remain hands-off; safe defaults apply

#### Details  
- **Environment:** Personal Developer  
- **Max Audience:** Personal / Small Workgroup

---

## Yellow Zone — Guided Development Zone

The Yellow Zone applies to agents that have grown beyond personal use and require IT collaboration. These agents may connect to external data sources, serve an entire department, or operate in trial or sandbox environments as they mature. Makers retain primary build responsibility, but IT guidance, custom DLP policy, and active oversight are introduced to ensure safe scaling before broader deployment.

### An agent lands in the **YELLOW ZONE** when:  
- Moving beyond personal Developer environments into Trial, Sandbox, or limited Production  
- Requires connectors or external actions beyond M365-native data  
- Sharing expands to a department or team (~up to 99 users)  
- Maker leads development but requires IT guidance or approval  
- Custom DLP policies or richer connector access is needed  
- Agent is transitioning from experimentation to departmental use  
- IT oversight is active but maker retains build responsibility

#### Details  
- **Environment:** Trial / Sandbox / Limited Prod  
- **Max Audience:** Department / ~99 Users

---

## Red Zone — IT Managed / Enterprise Zone

The Red Zone covers enterprise-grade agents that require the highest level of governance, security review, and lifecycle management. These agents are deployed tenant-wide, published to the organizational agent catalog, or handle sensitive and regulated data. IT owns the full build, test, and deployment pipeline, and all agents must pass mandatory privacy, responsible AI, and security reviews before going live.

### An agent lands in the **RED ZONE** when:  
- Targeting enterprise-wide or tenant-wide deployment  
- Will be published to the organizational agent catalog  
- Accesses sensitive data, uses multi-agent orchestration, or has autonomous actions  
- Requires full ALM (Dev → Test → Prod pipeline)  
- IT owns the full build and management lifecycle  
- Must pass Privacy, RAI, SDL, Threat Modeling, and Accessibility reviews  
- Professional developers or IT-approved makers only  
- Connector requests require formal IT approval

#### Details  
- **Environment:** IT-Provisioned Production  
- **Audience:** Enterprise-Wide / Tenant Catalog

---

## Decision Guide — Which Zone Is Right?

| Criteria                         | Zone   | Action Required                   |
|---------------------------------|--------|---------------------------------|
| Personal use, M365 data only     | GREEN  | Build freely in Developer Env   |
| Sharing with your team (~10 people) | GREEN  | Standard sharing, no approval   |
| Need an external API connector   | YELLOW | Request IT guidance              |
| Sharing with 50+ users in your dept | YELLOW | Notify IT, apply DLP policy      |
| Publishing org-wide or to catalog| RED    | IT approval required             |
| Autonomous agent with write actions | RED    | Full ALM + security review       |
| Accessing sensitive/regulated data | RED    | Privacy & RAI review required     |

---

> **Note:** Zone classification is not permanent. As an agent’s scope, audience, or capabilities evolve, its zone designation should be re-evaluated. Contact your Copilot Studio governance team for re-classification guidance.
