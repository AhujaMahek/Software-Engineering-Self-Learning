# Self-Learning Activity(I) — Software Engineering and Architecture 

# 1. DevOps

## 1.1 Introduction

DevOps combines culture, practices, automation, and tools to improve collaboration between development and operations. It replaces the traditional separation of "build" and "run" teams with shared ownership, continuous feedback, and frequent, automated delivery — aiming for faster releases without sacrificing quality or stability.

**Reference:** AWS, *What is DevOps?*

## 1.2 Principles

- **Collaboration & Communication** across development, operations, and security teams.
- **Automation** of repetitive build, test, and deployment tasks.
- **Continuous Integration and Continuous Delivery** for frequent and reliable software delivery.
- **Continuous Monitoring and Feedback** to identify problems and improve systems.
- **Shared Responsibility and Continuous Improvement** across the software lifecycle.
- **Security Integration (DevSecOps)** by incorporating security throughout the development lifecycle.

## 1.3 Lifecycle

The DevOps lifecycle is a continuous loop:

**Plan → Code → Build → Test → Release → Deploy → Operate → Monitor → Feedback → Plan**

This continuous cycle allows teams to repeatedly develop, deliver, monitor, and improve software.

## 1.4 DevOps Practices

- **Continuous Integration (CI)** — frequently merge and test code.
- **Continuous Delivery (CD)** — keep software in a release-ready state.
- **Continuous Deployment** — automatically deploy changes that pass all required checks.
- **Infrastructure as Code (IaC)** — manage infrastructure through version-controlled configuration.
- **Automated Testing** — verify functionality without repetitive manual effort.
- **Continuous Monitoring** — track application and infrastructure health.
- **Version Control** — track and manage changes to source code.
- **Configuration Management** — maintain consistent system configurations.
- **Containerization** — package applications and their dependencies into consistent environments.

## 1.5 CI/CD Summary

- **CI:** Frequently integrate and test code.
- **Continuous Delivery:** Keep software release-ready through automated build, test, and package steps.
- **Continuous Deployment:** Automatically deploy validated changes to production without a manual release gate.

## 1.6 Benefits of DevOps

- Faster and more frequent software delivery.
- Improved collaboration across teams.
- Better software quality through early defect detection.
- Increased reliability through standardized automation.
- Faster problem resolution through continuous monitoring.
- Better scalability and stronger security through DevSecOps practices.

## 1.7 DevOps Tools

| Category | Purpose | Examples |
|---|---|---|
| Version Control | Track source-code changes | Git, GitHub, GitLab |
| Project Management | Plan and track work | Jira, Azure Boards |
| CI/CD | Automate build, test, and delivery | Jenkins, GitHub Actions |
| Containers | Package applications and dependencies | Docker, Kubernetes |
| Infrastructure as Code | Manage infrastructure as code | Terraform, CloudFormation |
| Configuration Management | Automate configuration | Ansible |
| Monitoring | Track applications and infrastructure | Prometheus, Grafana |
| Cloud | Provide scalable infrastructure | AWS, Azure, Google Cloud |

# 2. JIRA

JIRA, developed by Atlassian, is a project management and issue-tracking tool built for Agile teams using methodologies such as Scrum and Kanban. It is used to manage requirements, user stories, tasks, bugs, backlogs, and sprints through boards, workflows, dashboards, and reports.

**Reference:** Atlassian, *Introduction to Jira*

### Features of JIRA

- Issue tracking.
- Backlog and sprint management.
- Scrum and Kanban boards.
- Customizable workflows.
- Reports and dashboards.
- Integration with other development tools.

### JIRA in Agile Project Management

A typical Agile workflow in JIRA is:

**Product Backlog → Sprint Planning → Sprint → Development & Testing → Review → Done**

### JIRA Workflow

**Backlog → To Do → In Progress → In Review → Testing → Done**

### Advantages of JIRA

- Centralized project management.
- Strong Agile support.
- Customizable workflows.
- Good project visibility.
- Broad integration capabilities.

### Limitations of JIRA

- Learning curve for new users.
- Complex configuration.
- May be excessive for very small teams.
- Requires administration and maintenance.
- Cost considerations depending on the plan and requirements.

# 3. Agile vs DevOps

Agile is an iterative approach to building software in small increments or sprints with frequent feedback and adaptability to change. DevOps combines development and operations practices such as automation, CI/CD, and monitoring to deliver software faster and more reliably.

They are complementary approaches:

- **Agile** helps teams build the right software.
- **DevOps** helps teams deliver and operate it efficiently.

**Reference:** Atlassian, *Agile vs DevOps*

## Agile vs DevOps Comparison

| Parameter | Agile | DevOps |
|---|---|---|
| **Focus** | Iterative development | End-to-end delivery and operations |
| **Scope** | Development and project management | Development, testing, deployment, operations, and monitoring |
| **Automation** | Useful, but not mandatory | Core component |
| **Deployment** | Usually after iterations | Frequent or continuous |
| **Monitoring** | Not central | Continuous practice |
| **Key Benefit** | Flexibility | Fast and repeatable delivery |

# 4. Case Study: JIRA and Asana in Real Projects

JIRA is development-oriented, providing features such as issue tracking, Agile boards, and sprint management. Asana is a general work-management platform used across both technical and non-technical teams.

## 4.1 JIRA — Twilio

Twilio uses JIRA across the organization. A two-person administration team manages JIRA for the whole company, while approximately 95% of projects are open to employees. This allows engineering, support, marketing, HR, and other teams to work using a transparent system.

**Reference:** Atlassian, *Teams at Twilio run on Jira*

## 4.2 Asana — Zoom

Before adopting Asana, teams at Zoom used a mixture of spreadsheets, email, and JIRA, with JIRA mainly being used by engineering teams. This created challenges in cross-team visibility.

Zoom now uses JIRA for engineering-related work and Asana for company-wide visibility. This allows marketing, IT, and leadership teams to monitor progress without relying heavily on manual reporting. The IT BYOD rollout achieved more than 90% enrollment through the use of Asana.

**Reference:** Asana, *Zoom Case Study*

## JIRA vs Asana

| Parameter | JIRA | Asana |
|---|---|---|
| **Orientation** | Software development | General project/work management |
| **Agile Support** | Strong Scrum/Kanban support | Supports Agile-style workflows |
| **Best For** | Software teams | Cross-functional teams |
| **Learning Curve** | Higher | Easier |

### Observation

Twilio uses JIRA alone because much of its work is technical, whereas Zoom uses Asana along with JIRA to provide non-engineering teams with greater visibility.

The appropriate choice depends on how technical the work is and how many teams require shared project visibility.

# 5. User Stories and Acceptance Criteria

A **user story** states a requirement from the user's perspective.

The standard format is:

> **As a [user], I want [goal], so that [benefit].**

### Example

> As a customer, I want to search products by name so that I can find what I need quickly.

## 5.1 INVEST Principles

| Principle | Meaning |
|---|---|
| **Independent** | The story should be as independent as possible from other stories. |
| **Negotiable** | The story should not unnecessarily prescribe the implementation. |
| **Valuable** | The story should provide clear value to the user. |
| **Estimable** | The development team should be able to estimate the effort. |
| **Small** | The story should be small enough to complete within a reasonable iteration. |
| **Testable** | The story should have clear conditions for verification. |

**Reference:** Atlassian, *User Stories With Examples and a Template*

## 5.2 Acceptance Criteria

Acceptance criteria are the conditions a user story must satisfy to be considered complete or "done."

They are commonly written using the **Given/When/Then** format.

### Login Example

- **Given** a registered account, **When** valid credentials are entered, **Then** login succeeds.
- **Given** an incorrect password, **When** the login form is submitted, **Then** an appropriate error message is shown.

**Reference:** Atlassian, *What is Acceptance Criteria?*

### Types of Acceptance Criteria

1. **Scenario-based** — Uses the Given/When/Then format.
2. **Rule-based** — Defines rules or conditions the system must satisfy.
3. **Checklist-based** — Provides a list of conditions that must be completed.

## 5.3 Example — Product Search

**User Story:**

> As a customer, I want to search for products by keyword so that I can quickly find products I'm interested in.

### Acceptance Criteria

- The user can enter a search keyword.
- The system displays matching products.
- A clear message is shown when no matching products are found.

## 5.4 Good vs Poor User Story

**Poor User Story:**

> Create a search API using a database query.

This describes an implementation rather than a user requirement.

**Better User Story:**

> As a customer, I want to search for products by keyword so that I can quickly find the products I need.

The better version identifies the **user, goal, and value** while leaving implementation details to the development team.

# 6. Advanced Requirement Elicitation

## 6.1 Interviews

Interviews are structured, semi-structured, or unstructured discussions with stakeholders to understand their needs, problems, expectations, and existing processes.

### Advantages

- Direct interaction with stakeholders.
- Detailed information can be collected.
- Immediate clarification is possible.

### Limitations

- Can be time-consuming.
- Responses can be incomplete or subjective.

### Example

For a hospital management system, analysts can interview doctors, nurses, and reception staff to understand how appointments, patient records, and other activities are handled.

## 6.2 Ethnography

Ethnography involves observing users in their real working environment to understand what they actually do rather than only what they report doing.

### Advantages

- Reveals hidden requirements.
- Helps identify real workflows.
- Shows how users actually interact with systems.

### Limitations

- Can be time-intensive.
- The presence of an observer may affect user behavior.

### Example

For a hospital management system, an analyst can observe nurses recording patient information during a normal shift to identify practical requirements and workflow problems.

## 6.3 Comparison

| Parameter | Interviews | Ethnography |
|---|---|---|
| **Main Approach** | Discussion with stakeholders | Observation of users |
| **Information Source** | What stakeholders say | What users actually do |
| **Hidden Requirements** | May not always reveal them | More likely to reveal them |
| **Time Required** | Generally lower | Generally higher |
| **Best Used For** | Opinions, expectations, and stated requirements | Real workflows and user behavior |
| **Main Challenge** | Incomplete or subjective responses | Time and interpretation |

Interviews capture **what stakeholders say they do**, while ethnography captures **what users actually do**. Using both techniques together provides a more complete understanding of requirements.

# 7. Requirement Traceability Matrix (RTM)

A **Requirement Traceability Matrix (RTM)** maps requirements to design, implementation, and test artifacts.

The basic relationship is:

**Requirement → Design → Implementation → Test Case → Test Result**

An RTM helps ensure that every requirement is covered and tested. It also supports impact analysis when requirements change.

## 7.1 Sample RTM

| Req ID | Requirement | Design Ref. | Implementation | Test Case | Status |
|---|---|---|---|---|---|
| REQ-01 | Register account | User Management | Registration Module | TC-01 | Tested |
| REQ-02 | Log in securely | Auth Module | Login Module | TC-02 | Tested |
| REQ-03 | Search products | Search Module | Search Module | TC-03 | Tested |
| REQ-04 | Add to cart | Cart Module | Cart Module | TC-04 | Implemented |
| REQ-05 | Place order | Order Management | Order Module | TC-05 | Implemented |
| REQ-06 | Order confirmation | Notification | Notification Module | TC-06 | Planned |

# 8. Requirement Management Tools

IBM DOORS is a requirements management tool for capturing, organizing, tracing, and managing requirements across large and complex projects with strict traceability and change-control needs.

**Reference:** IBM, *Engineering Requirements Management DOORS Next Documentation*

## Requirement Management Tools Comparison

| Tool | Purpose |
|---|---|
| **IBM DOORS** | Requirements management and traceability for complex projects |
| **Jama Connect** | Requirements, risk, and traceability management |
| **Siemens Polarion** | Requirements and Application Lifecycle Management |
| **Azure DevOps** | Work-item, requirement, development, and test management |
| **Jira** | Agile project management, issue tracking, and requirement-related work |

# 9. Conclusion

This activity covered DevOps, JIRA, Agile vs DevOps, a JIRA/Asana case study involving Twilio and Zoom, effective user stories and acceptance criteria using the INVEST principles, advanced requirement elicitation techniques such as interviews and ethnography, the Requirement Traceability Matrix (RTM), and requirement management tools such as IBM DOORS.

Together, these concepts demonstrate how Agile, DevOps, project management tools, and disciplined requirements engineering support reliable and efficient software delivery.

# 10. References

1. **AWS**, *What is DevOps?*  
   https://aws.amazon.com/devops/what-is-devops/

2. **Atlassian**, *Introduction to Jira*  
   https://www.atlassian.com/software/jira/guides

3. **Atlassian**, *Agile vs DevOps*  
   https://www.atlassian.com/devops/what-is-devops/agile-vs-devops

4. **Atlassian**, *User Stories With Examples and a Template*  
   https://www.atlassian.com/agile/project-management/user-stories

5. **Atlassian**, *What is Acceptance Criteria?*  
   https://www.atlassian.com/work-management/project-management/acceptance-criteria

6. **Atlassian**, *Teams at Twilio run on Jira*  
   https://www.atlassian.com/software/jira/great-teams/twilio

7. **Asana**, *Zoom Case Study*  
   https://asana.com/case-study/zoom

8. **IBM**, *Engineering Requirements Management DOORS Next Documentation*  
   https://www.ibm.com/docs/en/engineering-lifecycle-management-suite/doors-next