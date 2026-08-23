**PHASE1 - Project Foundation**

**Company:** Devv Global

**Type:** Technology / IT services company

**Project:** IT Service Request Management System



**Business Context**



"Devv Global" is a mid-sized technology services company with approximately 500 employees across multiple departments.



The company has an internal IT Support team responsible for:



1. Hardware/software issues
2. Access and account requests
3. Network/connectivity problems
4. Application support
5. General IT service requests



**Current situation**



Employees currently raise IT requests through email, Teams messages, phone calls, or directly approaching IT staff.



There is no centralized request-management process.



**Problem statement**:



Devv Global's decentralized IT support process causes requests to be missed, inconsistently prioritized, difficult to track, and dependent on manual follow-ups. The IT team also lacks centralized visibility into request volume, status, ownership, and SLA performance.



**Business impact**:



Missed/delayed requests

Longer resolution times

Poor employee experience

Inefficient IT workload management

Limited management visibility

No reliable SLA tracking



**Project Objectives**



The project aims to:



**Centralize** employee IT service requests through a single request-management process.

**Improve prioritization and assignment** of requests based on category and urgency.

Provide request visibility so employees can track status without repeated follow-ups.

**Improve SLA monitoring** by giving the IT team visibility into request ownership and resolution timelines.

**Improve management visibility** through basic reporting on request volume, status, priority, and resolution performance.



**Success Criteria**

We'll measure the proposed solution against these targets:



100% of IT requests are recorded in the centralized system.

Employees can view the status of their requests.

Every request has an assigned category, priority, and owner.

IT management can monitor open requests and SLA status.

Request history is available for tracking and reporting.



**In Scope**

Employee IT service-request submission

Request categorization

Priority assignment

IT assignment/ownership

Request status tracking

Request updates and resolution

SLA tracking

Basic request reporting

Notifications/status communication

**Out of Scope**

Actual IT infrastructure implementation

Hardware procurement

Payroll/HR requests

Financial processes

Advanced AI chatbot

Full IT asset-management system

Detailed production deployment



**Stakeholders**



| **Stakeholder**               | **Role**                    | **Main Need**                            |

| ------------------------- | ----------------------- | ------------------------------------ |

| \*\*Employees\*\*             | IT service requesters   | Easy submission + status tracking    |

| \*\*IT Support Agents\*\*     | Resolve requests        | Clear queue, priority, ownership     |

| \*\*IT Support Manager\*\*    | Manage IT operations    | SLA + workload visibility            |

| \*\*Department Managers\*\*   | Business stakeholders   | Minimize employee downtime           |

| \*\*HR/Admin\*\*              | Supporting stakeholder  | Employee/access-related coordination |

| \*\*Project/Product Owner\*\* | Business decision-maker | Business value + successful delivery |



**Stakeholder Needs**

**Employees**

Simple request submission

Request tracking

Status notifications

Faster resolution

**IT Support**

Centralized queue

Categorization and prioritization

Clear ownership

Complete request history

**IT Manager**

SLA monitoring

Workload visibility

Performance reporting

**Department Managers**

Reduced employee downtime

Visibility into critical issues

**HR/Admin**

Efficient coordination for access/account-related requests

**Project/Product Owner**

Improved IT service efficiency

Measurable business value





**Assumptions**

Employees have company credentials.

IT Support staff will use the centralized system.

Requests can be categorized using predefined categories.

SLA rules can be defined by priority.

Email/system notifications are available.

**Constraints**

Project focuses on an MVP.

Existing IT infrastructure is not being redesigned.

No actual production deployment is required.

API testing will focus only on functionality relevant to this case study.



**Project Scope Summary**

Business Problem → Centralized IT Service Request Management



Users → Employees + IT Support



Core capabilities → Submit → Categorize → Prioritize → Assign → Track → Resolve → Monitor



Project objective → Improve visibility, efficiency, SLA management, and employee experience.





**PHASE3 - Requirements Definition**

AS-IS Gap Analysis



Now we translate the BPMN into BA findings.



Step 14A — Process Gaps



Use these as our finalized gaps:



ID	Gap	Root Cause	Business Impact

G1	Multiple request channels	No centralized intake mechanism	Requests may be missed

G2	Manual request recording	No standardized ticketing process	Incomplete/inconsistent information

G3	Manual prioritization	No defined priority rules	Inconsistent handling of urgent issues

G4	Unclear ownership	No centralized assignment mechanism	Delayed resolution

G5	Manual status follow-ups	Employees lack self-service tracking	Time wasted on follow-ups

G6	Limited SLA visibility	No centralized SLA tracking	Management cannot monitor performance effectively

G7	Limited reporting	Request data is fragmented	Poor workload and trend visibility

Step 14B — Improvement Opportunities



These gaps point directly toward our future solution:



Centralized intake

→ One place to submit requests



Standardized request information

→ Categories + required details



Defined prioritization

→ Priority rules based on urgency/impact



Clear ownership

→ Assign requests to IT Support agents



Self-service tracking

→ Employee can see request status



SLA monitoring

→ Track response/resolution against defined targets



Reporting

→ Request volume, priority, status, resolution time



Important BA connection



This is where our project starts becoming more than a BPMN exercise:



AS-IS process → Gaps → Requirements → TO-BE process → User Stories → Jira implementation



Every major requirement we create next should be traceable back to one or more of these gaps.



Business Requirements



Copy these to your working notes:



BR1. The system shall provide a centralized channel for employees to submit IT service requests.



BR2. The system shall capture standardized request information, including category, description, urgency, and requester details.



BR3. The system shall support request prioritization based on defined business rules.



BR4. The system shall allow IT Support to assign ownership of requests.



BR5. The system shall allow employees to view the status of their requests.



BR6. The system shall support SLA tracking for IT service requests.



BR7. The system shall provide basic reporting on request volume, status, priority, ownership, and resolution performance.



Functional Requirements



Add these to your notes:



FR1: Employees can submit an IT service request through the centralized system.

FR2: The system captures requester, category, description, urgency, and submission date/time.

FR3: IT Support can view, categorize, prioritize, and assign requests.

FR4: The system maintains request statuses: New → Assigned → In Progress → Resolved → Closed.

FR5: Employees can view the current status and details of their submitted requests.

FR6: The system records request timestamps needed for SLA monitoring.

FR7: The system provides basic reports for request volume, status, priority, ownership, and resolution time.

FR8: The system sends notifications when key request events occur, such as assignment, status change, or resolution.



Non-Functional Requirements + Business Rules

NFRs

NFR1 — Usability: Employees should be able to submit a request with minimal steps.

NFR2 — Performance: Request submission and status updates should respond within 3 seconds under normal load.

NFR3 — Availability: System should be available during normal business operations.

NFR4 — Security: Only authenticated employees and authorized IT staff can access relevant request information.

NFR5 — Auditability: Request status, assignment, and key updates should be recorded.

NFR6 — Scalability: The solution should support growth in employees and request volume without major redesign.

Business Rules

BRULE1: Every request must have a category and description.

BRULE2: Every request must have a priority.

BRULE3: Every request must have an owner once assigned.

BRULE4: Priority is determined using impact + urgency.

BRULE5: Only authorized IT Support staff can change assignment or priority.

BRULE6: A request can be closed only after it has been resolved.

BRULE7: SLA targets depend on request priority.



User Stories + Acceptance Criteria



Keep this to 8 core stories.



US1 — Submit Request



As an employee, I want to submit an IT service request so that I can get IT support.



Acceptance criteria



Requester details are captured automatically.

Category and description are mandatory.

Successful submission generates a unique request ID.

US2 — Categorize Request



As an IT Support Agent, I want to categorize requests so that they can be handled appropriately.



Agent can select a predefined category.

Category is saved with the request.

Request cannot proceed without a category.

US3 — Prioritize Request



As an IT Support Agent, I want to prioritize requests based on impact and urgency so that critical issues are handled first.



Impact and urgency can be recorded.

System determines/records the resulting priority.

Priority is visible to IT Support.

US4 — Assign Request



As an IT Support Manager, I want to assign requests to IT Support Agents so that every request has clear ownership.



Manager can select an available agent.

Assigned agent is recorded.

Assignment is visible in the request.

US5 — Track Request



As an employee, I want to view my request status so that I know its progress without contacting IT.



Employee can view submitted requests.

Current status is displayed.

Request ID and key details are visible.

US6 — Update Request



As an IT Support Agent, I want to update request status so that the request lifecycle is accurately tracked.



Agent can update status.

Allowed statuses follow the defined workflow.

Status changes are recorded.

US7 — Monitor SLA



As an IT Support Manager, I want to monitor SLA performance so that delayed requests can be identified and addressed.



SLA target is associated with priority.

Current SLA status is visible.

Overdue requests can be identified.

US8 — View Reports



As an IT Support Manager, I want to view basic service-request reports so that I can monitor workload and performance.



Reports show request volume.

Reports can show status, priority, ownership, and resolution time.

Data can be filtered for meaningful analysis.



Prioritization + Traceability

MoSCoW Prioritization

Story	Priority

US1 — Submit Request	Must Have

US2 — Categorize Request	Must Have

US3 — Prioritize Request	Must Have

US4 — Assign Request	Must Have

US5 — Track Request	Must Have

US6 — Update Request	Must Have

US7 — Monitor SLA	Should Have

US8 — View Reports	Should Have



MVP = US1–US6.



Requirement → Story Traceability

BR1 → US1

BR2 → US1, US2

BR3 → US3

BR4 → US4

BR5 → US5

BR6 → US7

BR7 → US8



**PHASE4 - Solution Definition**

TO-BE Solution Definition

Proposed Solution



Devv Global will introduce a centralized IT Service Request Management System.



Core flow:



Employee submits request

→ System captures required details

→ IT Support categorizes request

→ Priority determined using impact + urgency

→ Request assigned to IT Support Agent

→ Agent works on request

→ Employee receives status updates

→ Issue resolved

→ Request closed

→ SLA/reporting data captured



Key improvements

AS-IS	TO-BE

Multiple channels	Centralized request portal

Manual recording	Structured request creation

Inconsistent priority	Defined priority rules

Unclear ownership	Assigned IT agent

Manual follow-ups	Self-service status tracking

Limited SLA visibility	SLA monitoring

Fragmented information	Centralized reporting



AS-IS vs TO-BE Improvement Analysis



Add this to your working notes:



Area	AS-IS	TO-BE	Improvement

Request intake	Multiple channels	Centralized portal	Reduced missed requests

Request information	Manual/inconsistent	Structured fields	Better data quality

Priority	Manual	Impact + urgency	Consistent prioritization

Ownership	Unclear	Assigned agent	Clear accountability

Status	Manual follow-ups	Self-service tracking	Better visibility

SLA	Limited visibility	SLA monitoring	Better control

Reporting	Fragmented	Centralized data	Better decision-making



Business outcome



The TO-BE process creates a standardized, centralized and trackable IT service-request lifecycle, addressing the major gaps identified in the AS-IS analysis.





**PHASE5 -**

