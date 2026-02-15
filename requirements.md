# AccessAI (AI Sarthi)
## Software Requirements Specification (SRS)

**AWS Hackathon 2025**  
**Theme:** Topic-06 – AI for Communities, Access & Public Impact  

---
## Executive Summary

AccessAI (AI Saathi) is an AI-powered, voice-first, multilingual public access platform designed to improve how communities discover, understand, and navigate public information, resources, and opportunities.

Despite large-scale digitization of public services, access remains unequal due to fragmented portals, text-heavy interfaces, language barriers, low digital literacy, and unreliable connectivity. AccessAI addresses this gap by acting as a **human-centric AI access layer** between communities and public systems, enabling guided, contextual, and inclusive interaction.

The system is architected using **AWS cloud-native services**, ensuring security, scalability, and real-world deployability with measurable public impact.

---

## Document Control

| Attribute | Details |
|---------|---------|
| Product Name | AccessAI (AI Sarthi) |
| Team Name | TECH B4T |
| Hackathon | AWS Hackathon 2026 |
| Theme | AI for Communities, Access & Public Impact |
| Document Type | Software Requirements Specification |
| Version | 1.0 |
| Status | Final |
| Last Updated | February 2026 |

---

## Table of Contents

1. Executive Summary  
2. Purpose of the Document  
3. Scope of the System  
4. Background & Public Context  
5. Problem Landscape  
6. Goals & Strategic Objectives  
7. Stakeholders  
8. User Personas  
9. User Needs & Usage Scenarios  
10. System Overview  
11. Functional Requirements  
12. Non-Functional Requirements  
13. Accessibility Requirements  
14. Personalisation & Context Handling  
15. Low-Bandwidth & Intermittent Connectivity Considerations  
16. Security & Privacy Requirements  
17. Ethical & Responsible AI Principles  
18. Data Handling & Governance  
19. Assumptions  
20. Constraints  
21. Risks & Mitigation Strategies  
22. Success Metrics & Evaluation Criteria  
23. Compliance with Hackathon Theme  
24. Future Expandability & Roadmap  
25. Conclusion  

---

## 1. Executive Summary

AccessAI is an AI-powered, voice-first public access system designed to improve how communities interact with public information, resources, and opportunities. While public services have been widely digitized, **access remains uneven and exclusionary** due to fragmented portals, text-heavy interfaces, language barriers, low digital literacy, and unreliable connectivity.

AccessAI addresses this structural gap by acting as a **human-centric access layer**, enabling citizens to express needs naturally and receive guided, contextual assistance. The system is designed specifically for rural, elderly, and digitally underserved populations, ensuring that public services are not only available but **actually usable in real-world conditions**.

---

## 2. Purpose of the Document

This document defines the complete software requirements for AccessAI and serves multiple purposes:
- Establishes a formal requirements baseline
- Demonstrates system maturity and feasibility
- Acts as a judging artifact for AWS Hackathon 2025
- Ensures traceability between community needs and system capabilities

The document emphasizes **access enablement**, not policy creation or enforcement.

---

## 3. Scope of the System

### 3.1 In Scope

AccessAI supports:
- Discovery of public schemes and services
- Explanation of eligibility and requirements
- Step-by-step procedural guidance
- Voice-first and multilingual interaction
- Usage in low-bandwidth and intermittent connectivity environments
- Assisted access through facilitators such as CSCs and NGOs

### 3.2 Out of Scope

The system does not:
- Approve or reject applications
- Perform financial transactions
- Modify public policy
- Replace official government portals

---

## 4. Background & Public Context

Public institutions have invested significantly in digital platforms to improve service delivery. However, most systems mirror paper-based processes, resulting in interfaces that assume:
- High digital literacy
- Proficiency in official languages
- Stable internet connectivity
- Independent error recovery

These assumptions systematically exclude large segments of the population. AccessAI focuses on redesigning **access**, not infrastructure, ensuring that communities can engage with public systems meaningfully.

---

## 5. Problem Landscape

Citizens approach public systems with **life needs**, not administrative knowledge. These needs may include healthcare support, financial assistance, education, skills training, or employment opportunities.

Existing platforms require users to:
- Know scheme names
- Identify responsible departments
- Navigate multi-step workflows
- Interpret complex documentation

This mismatch leads to confusion, abandonment, and dependence on intermediaries, undermining public impact.

---

## 6. Goals & Strategic Objectives

### Primary Goals
- Reduce structural access barriers
- Improve service awareness and adoption
- Enable inclusive participation
- Deliver real-world societal impact

### Strategic Objectives
- Design for low digital literacy
- Ensure ethical and non-intrusive personalisation
- Support scalable public deployment
- Maintain institutional neutrality and trust

---

## 7. Stakeholders

| Stakeholder | Role & Interest |
|------------|----------------|
| Citizens | Simple, reliable access to services |
| Communities | Equity, inclusion, empowerment |
| Public Institutions | Improved reach and adoption |
| NGOs / CSCs | Assisted access enablement |
| Hackathon Judges | Impact, feasibility, alignment |

---

## 8. User Personas

### 8.1 Rural Citizen
Often uses mobile internet with intermittent connectivity, prefers voice interaction, and may be unfamiliar with digital portals.

### 8.2 Elderly User
Requires simplified explanations, assistive interaction, and reassurance during multi-step processes.

### 8.3 Assisted Access Facilitator
Supports multiple users, requires structured guidance flows, and acts as a bridge between citizens and systems.

---

## 9. User Needs & Usage Scenarios

Users need to:
- Discover services without knowing official terminology
- Understand eligibility clearly and confidently
- Avoid complex forms at early stages
- Receive step-by-step guidance
- Resume interactions after interruptions
- Feel confident and supported throughout the journey

---

## 10. System Overview

AccessAI functions as a **conversational interface layer** that sits between citizens and public information systems. It interprets natural language input, identifies relevant services, and delivers contextual guidance without replacing official platforms.

---

## 11. Functional Requirements

| ID | Requirement |
|----|------------|
| FR-01 | Support voice-first interaction |
| FR-02 | Support text-based interaction |
| FR-03 | Support regional and local languages |
| FR-04 | Understand user intent via NLP |
| FR-05 | Provide personalised, context-aware guidance |
| FR-06 | Explain eligibility in simple language |
| FR-07 | Provide step-by-step process guidance |
| FR-08 | Operate reliably in low-bandwidth conditions |
| FR-09 | Support assisted access usage |

---

## 12. Non-Functional Requirements

### Performance
The system shall deliver low-latency responses and support concurrent users without degradation.

### Reliability
The system shall handle errors gracefully, allow session recovery, and avoid penalizing users for interruptions.

### Scalability
The system shall be cloud-native and horizontally scalable to support regional or national deployment.

### Maintainability
The system shall be modular, configurable, and extensible.

---

## 13. Accessibility Requirements

Accessibility is a core requirement, not an add-on:
- Voice-first interaction by default
- Simple, non-technical language
- Designed for low digital literacy users
- Compatible with assistive access scenarios

---

## 14. Personalisation & Context Handling

Personalisation is strictly ethical and limited to interaction context:
- Based on user input, location, and conversation flow
- No behavioral profiling
- No sensitive attribute inference
- Transparent and explainable guidance

---

## 15. Low-Bandwidth & Intermittent Connectivity Considerations

The system shall:
- Optimize payload size
- Minimize repeated data transfer
- Tolerate session interruptions
- Provide clear recovery paths

---

## 16. Security & Privacy Requirements

- Privacy-by-design architecture
- Minimal data collection
- Secure communication channels
- No long-term storage of personal data
- No automated decision-making

---

## 17. Ethical & Responsible AI Principles

AccessAI adheres to:
- Human-centric AI usage
- Bias avoidance
- Neutral and factual responses
- Preservation of user agency
- Transparency in limitations

---

## 18. Data Handling & Governance

- Contextual data used only during interaction
- No long-term personal data retention
- Aggregated, anonymized insights only
- Clear governance boundaries

---

## 19. Assumptions

- Users may not know scheme names
- Connectivity may be unstable
- Digital skills vary significantly
- Public data sources may differ by region

---

## 20. Constraints

- Informational guidance only
- Dependent on accuracy of public data
- Regional policy variations apply
- No replacement of official systems

---

## 21. Risks & Mitigation Strategies

| Risk | Mitigation |
|----|-----------|
| User confusion | Guided conversational flow |
| Connectivity loss | Session tolerance |
| Data mismatch | Transparent communication |

---

## 22. Success Metrics & Evaluation Criteria

- Increased awareness of services
- Reduced drop-off rates
- Improved completion confidence
- Higher inclusion of underserved users
- Positive community feedback

---

## 23. Compliance with Hackathon Theme

AccessAI directly supports:
- Civic information and public service assistance
- Community-level access enablement
- Voice-first, low-bandwidth AI solutions
- Inclusion and real-world societal impact

---

## 24. Future Expandability & Roadmap

- Integration with healthcare and welfare domains
- Skill development and employment modules
- Omnichannel access (voice, text, assisted)
- Deeper localization support

---

## 25. Conclusion

AccessAI reimagines how communities interact with public systems by replacing complexity with clarity and portals with conversations.
## Final Summary

This Software Requirements Specification defines the functional, non-functional, accessibility, security, and ethical requirements for **AccessAI (AI Saathi)** — an AI-powered public-service access platform aligned with the **AI for Communities, Access & Public Impact** theme.

The requirements are intentionally designed to address real-world access constraints faced by communities, including language diversity, low digital literacy, accessibility needs, and unreliable connectivity. Rather than optimizing for feature complexity, the system prioritizes **usability, inclusivity, and guided understanding**, ensuring that public information and opportunities are not only available but genuinely accessible.

Key requirement principles include:
- **Voice-first and multilingual interaction** to reduce literacy and language barriers  
- **Context-aware, ethical personalisation** to support users without profiling or bias  
- **Low-bandwidth tolerance and resilience** to function in constrained environments  
- **Privacy-by-design and security-first architecture** suitable for public-scale deployment  
- **Cloud-native scalability** to support phased rollout from pilot to national adoption  

The requirements explicitly avoid automated decision-making, transactional authority, or policy enforcement, preserving institutional neutrality and user trust. Instead, AccessAI functions as a **human-centric access layer** that bridges the gap between public systems and community needs.

This document establishes a clear, implementable baseline for building an AI system that delivers **measurable societal impact**, supports equitable access, and aligns with the expectations of public institutions and large-scale governance ecosystems.

**AccessAI is defined not as a product feature, but as foundational public-access infrastructure—designed to scale responsibly and inclusively.**

**This is AI designed for communities, access, and real public impact.**