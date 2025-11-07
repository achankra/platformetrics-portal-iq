# Portal IQ: Platform Engineering Tool Comparison

## Overview

**Portal IQ** is a structured decision-making framework for evaluating Internal Developer Portals (IDPs) and engineering platforms. It helps technology leaders choose the right combination of tools that improve developer experience, operational efficiency, and business value.

You can access the framework here [Portal IQ](https://portal-iq.platformetrics.com), but please read the entire document to understand how to use it

Rather than treating every platform tool as a “DevOps solution,” Portal IQ organizes the landscape into **platform planes**, **capabilities**, and **outcomes**, aligning these dimensions with your organization’s unique context.

A detailed analysis of the [Portal IQ Approach](APPROACH.md) is available for your review, well, only if you are curious about it.

---

## What You Will Compare

Portal IQ evaluates **eight leading platform engineering solutions** across multiple dimensions to help you identify the best fit for your needs. You might ask, why these, and why not anything else? These are generally market leaders, and this is what we hear most from our clients. 

- [Backstage OSS](https://backstage.io)
- [Spotify Portal](https://backstage.spotify.com/)
- [Port](https://port.io)
- [Cortex](https://cortex.io)  
- [Harness IDP](https://harness.io)
- [OpsLevel](https://www.opslevel.com/)
- [Aviator](https://aviator.co)
- [Atlassian Compass](https://www.atlassian.com/software/compass)

These tools represent different approaches to enabling self-service, standardization, and insight-driven developer experiences.

Kindly do not die wondering why are IDPs (Internal Developer Platforms) not shown here. The reason is simple. IDPs != Dev Portals. If you are confused already, we urge you to get a copy of [Effective Platform Engineering](https://effectiveplatformengineering.com) and read chapter 10 for an authoritative analysis of this field of study.

---

## Homegrown Portal Option

Many organizations choose to build their own portal—typically using **Backstage OSS** or a custom framework—similar to Visit [Platformetrics Portal](https://portal.platformetrics.com) to learn more. 
A homegrown portal offers deep control and domain alignment but requires ongoing investment and expertise. We haven't included that in the study as your requirements might be very different. Expect the cost to be very high if you are building a custom, exhaustive portal. If you are going to build it anyway, you don't need any comparisons as its a philosophical decision.

### When a Homegrown Portal Works Best
- You need domain-specific workflows and deep customization.  
- Your platform team already maintains Backstage or a similar framework.  
- You require control over data, security, and roadmap priorities.

### Core Feature Priorities
1. **Service Catalog and Ownership** – A single source of truth for systems and teams.  
2. **Golden Paths** – Opinionated templates for creating new services and workflows.  
3. **Scorecards and Standards** – Lightweight health views before implementing full automation.  
4. **Integrations** – Start with version control, CI/CD, incidents, and cost tools.

### Complementing Homegrown Solutions
- **Port, OpsLevel, Cortex, Harness, and Compass** add workflow automation, maturity tracking, and governance.  
- **Aviator** enhances ownership and collaboration features.  
- **Spotify Portal for Backstage** simplifies setup, updates, and lifecycle management.

---

## Feature Comparison

| Feature | Homegrown (Backstage-style) | SaaS Portals (Port, OpsLevel, Cortex, Harness, Compass) | Specialized Tooling (Aviator) |
|----------|------------------------------|----------------------------------------------------------|-------------------------------|
| Time to first portal | Medium – depends on internal expertise | Fast – weeks with vendor support | N/A – adds capabilities on top |
| Customization depth | Very high – full code control | High – configurable via APIs | Medium – focused on ownership |
| Ongoing effort | High – requires a dedicated team | Medium – vendor-managed core | Low – minimal operational overhead |
| Ecosystem | Strong – broad plugin support | Strong – curated integrations | Focused – tight CI/CD integration |

Portal IQ helps prioritize whether to double down on a homegrown platform, adopt a SaaS solution, or use both strategically.

---

## Using Portal IQ

### Step 1: Define Your Team Size
Your team size determines whether to pursue a fully managed IDP or invest in a custom-built platform.

- **Small teams (≤50 developers):** Prefer turnkey SaaS tools for faster ROI.  
- **Larger organizations:** Benefit from custom portals that evolve alongside the platform team.

### Step 2: Choose Primary Outcomes
Identify what success means for your platform initiative:

- **Developer Experience (DevEx):** Reduce friction, increase autonomy, and improve onboarding.  
- **Operational Excellence:** Drive reliability, SLO maturity, and SRE alignment.  
- **Governance and Compliance:** Ensure consistency and clarity across teams.  
- **Cost and Efficiency:** Gain visibility into spend and platform utilization.

### Step 3: Map to Platform Planes
Portal IQ evaluates tools across six key planes:

1. Service Catalog and Ownership  
2. Golden Paths and Scaffolding  
3. Operations and Reliability  
4. Security and Governance  
5. Observability and Telemetry  
6. SEI and AI-Augmented Insights  

Each tool emphasizes a different combination of these capabilities.

### Step 4: Assess Fit
Compare tools based on:

- Platform plane coverage  
- Integration depth with your ecosystem  
- Implementation and operational effort  
- Pricing and scalability model  

---

## Key Evaluation Dimensions

### 1. Platform Plane Coverage
- Identify which capabilities are built-in versus integrated.  
- Understand whether the tool is catalog-first, workflow-first, or governance-first.  
- Evaluate how well multi-plane workflows are supported.

**Example:**  
Backstage excels at catalogs and golden paths. Cortex and OpsLevel are strongest in standards and maturity scoring.

---

### 2. Integration Depth
- CI/CD, SCM, incident management, observability, and cloud integration coverage.  
- Extensibility through APIs, webhooks, and plug-ins.  
- Compatibility with emerging SEI and AI-driven tools.

**Example:**  
Compass integrates tightly within Atlassian Cloud, while Harness IDP connects across its DevOps pipeline and cost suite.

---

### 3. Implementation and Operations
- Time-to-first-value (TTFV).  
- Ownership model (vendor-managed vs. platform-managed).  
- Ease of upgrades and experimentation.

 **Note:** A simpler, fast-moving platform that teams can actually maintain is more valuable than a sophisticated portal that no one can sustain.

---

### 4. Developer Experience
- UI/UX quality, discoverability, and navigation.  
- Self-service workflows, golden paths, and guardrails.  
- Impact on cognitive load and context switching.

---

### 5. Governance and Compliance
- Service health and maturity visibility.  
- Policy enforcement mechanisms.  
- Support for frameworks such as SOC2, PCI, and HIPAA.

---

### 6. AI and SEI Readiness
- Integration with Software Engineering Intelligence and observability data.  
- Support for AI copilots and automation workflows.  
- Extensibility for analytics and predictive insights.

Portal IQ anticipates a near future where internal portals act as **control planes for AI-assisted engineering ecosystems.**

---

## Evaluation by Persona

| Persona | Primary Focus |
|----------|----------------|
| **CTO / VP of Engineering** | Strategic alignment, ROI, risk, and modernization roadmap |
| **Platform / SRE Teams** | Integrations, automation, and golden path implementation |
| **Security and Compliance** | Auditability, policy enforcement, and access control |
| **Finance and Product** | Cost attribution, scalability, and investment visibility |

Each persona can weight criteria differently in Portal IQ to reach a balanced decision.

---

## Common Decision Scenarios

**Fast Time to Market**  
- *Best fit:* Port, OpsLevel, or Spotify Portal  
- *Trade-off:* Limited low-level customization  

**Maximum Customization**  
- *Best fit:* Backstage OSS  
- *Trade-off:* Requires engineering investment  

**Enterprise Compliance**  
- *Best fit:* Cortex, OpsLevel, Atlassian Compass  
- *Trade-off:* Higher cost and longer setup  

**Existing Ecosystem Alignment**  
- *Best fit:* Compass (Atlassian) or Harness IDP  
- *Trade-off:* Vendor lock-in  

**Cost-Conscious Teams**  
- *Best fit:* Port or Aviator, potentially layered over Backstage OSS  
- *Trade-off:* Increased internal maintenance as adoption grows  

---

## Deliverables

When configured, Portal IQ produces:

- A ranked list of suitable tools with pros and cons  
- An executive summary focused on business value  
- A detailed technical appendix for platform and SRE teams  

This structured approach helps teams avoid opinion-based “tool contests” and make decisions grounded in measurable outcomes.

---
## License

Portal IQ is released under the **MIT License**. See [LICENSE](./LICENSE) for details.

You are free to:
- Use Portal IQ for personal, commercial, or research purposes
- Modify and distribute the code
- Integrate it into your own products and services

We only ask for attribution when using or modifying Portal IQ.

---
## Code

Portal IQ code could be open-sourced soon. We are still working making a few additional changes.

---

## Conclusion

**Portal IQ** provides a consistent framework for evaluating, comparing, and implementing internal developer portals and platforms.  
By organizing choices around precise dimensions—platform planes, personas, and outcomes—it turns complexity into clarity and helps you invest wisely in developer experience.

---

## Attribution

Created by **Platformetrics** – an advisory and education firm focused on AI-augmented platform engineering, developer experience, and software delivery excellence.  
© 2025 Platformetrics. All rights reserved.
