# IT Service Request Management — Business Analysis Case Study

![Business Analysis](https://img.shields.io/badge/Focus-Business%20Analysis-2457A7)
![Requirements](https://img.shields.io/badge/Practice-Requirements%20Engineering-386CB0)
![Process Modelling](https://img.shields.io/badge/Practice-BPMN%20Process%20Modelling-4C8C72)
![Tools](https://img.shields.io/badge/Tools-Draw.io%20%7C%20Jira%20%7C%20Postman-6554C0)

An end-to-end, portfolio-based Business Analyst case study focused on analysing and improving an IT service request process. The work demonstrates how a business problem can be translated into documented requirements, process models, user stories, delivery work items, and API-level validation evidence.

> **Project type:** Independent learning case study using a simulated business scenario. It is not a live client implementation or production ITSM deployment.

## Business context

IT support requests can arrive through inconsistent channels, making it harder for employees and support teams to maintain a common view of request details, ownership, priority, and progress.

This case study explores a more structured service-request approach: capture requests consistently, define how they should be handled, make the process visible, and provide supporting requirements and test evidence.

## Business analysis approach

**Business problem → scope and requirements → AS-IS analysis → TO-BE process → user stories and acceptance criteria → Jira workflow → API testing evidence**

The work connects the business view with delivery-oriented artefacts:

- **Requirements analysis:** business, functional, and non-functional requirements.
- **Process analysis:** current-state and proposed process models, with improvement opportunities.
- **Requirements elaboration:** user stories and acceptance criteria.
- **Delivery support:** Jira epic, backlog items, priorities, and Kanban workflow.
- **System interaction awareness:** mock REST API requests and response checks using Postman.

## Process models

The diagrams below show the current-state process and the proposed process.

| AS-IS process | TO-BE process |
|---|---|
| ![AS-IS IT service request process](process-models/IT%20mgmt%20draws-AS-IS%20process.drawio.png) | ![TO-BE IT service request process](process-models/IT%20mgmt%20draws-TO-BE%20process.drawio.png) |

[Open the editable Draw.io source](process-models/IT%20mgmt%20draws.drawio).

## Key deliverables

| BA activity | Deliverable |
|---|---|
| Business and requirements definition | [Business Requirements Document (BRD)](requirements/IT-Service-Request-Management-BRD.pdf) |
| Requirements elaboration | [User Stories and Acceptance Criteria](user-stories/User-Stories-and-Acceptance-Criteria.pdf) |
| Process analysis | [AS-IS process](process-models/IT%20mgmt%20draws-AS-IS%20process.drawio.png) · [TO-BE process](process-models/IT%20mgmt%20draws-TO-BE%20process.drawio.png) |
| Agile delivery support | [Jira epic and user stories](jira/jira-epic-and-user-stories.png) · [Jira Kanban board](jira/jira-kanban-board.png) |
| API testing evidence | [Postman test results](api-testing/postman-api-test-results.png) · [Postman collection](api-testing/IT%20Service%20Request%20Management%20API.postman_collection.json) |
| Consolidated project report | [Business Analyst Case Study PDF](documentation/IT-Service-Request-Management-BA-Case-Study.pdf) |

## API testing scope

A mock REST API is used to practise common service-request operations and response validation.

| Method | Demonstrated operation | Expected response shown in project |
|---|---|---|
| GET | Retrieve a service request | 200 OK |
| POST | Create a service request | 201 Created |
| PUT | Update a service request | 200 OK |
| DELETE | Delete a service request | 200 OK |

The API component is a learning exercise for understanding request/response behaviour. It does not represent a production ITSM backend.

## Tools and techniques

- **Business analysis:** business problem framing, requirements documentation, user stories, acceptance criteria.
- **Process modelling:** Draw.io, BPMN-style process diagrams, AS-IS / TO-BE analysis.
- **Agile work management:** Jira epic, backlog items, prioritisation, and Kanban workflow.
- **API exploration:** Postman, REST methods, response checks.
- **Documentation and versioning:** PDF artefacts, Markdown, GitHub.

## Repository structure

```text
IT-Service-Request-Management-BA-Case-Study/
├── api-testing/
│   ├── IT Service Request Management API.postman_collection.json
│   └── postman-api-test-results.png
├── documentation/
│   └── IT-Service-Request-Management-BA-Case-Study.pdf
├── jira/
│   ├── jira-epic-and-user-stories.png
│   └── jira-kanban-board.png
├── process-models/
│   ├── IT mgmt draws.drawio
│   ├── IT mgmt draws-AS-IS process.drawio.png
│   └── IT mgmt draws-TO-BE process.drawio.png
├── requirements/
│   ├── IT-Service-Request-Management-BRD.pdf
│   └── Project_Working_Notes.md
└── user-stories/
    └── User-Stories-and-Acceptance-Criteria.pdf
```

## Outcome

This case study brings together core BA activities across the analysis-to-delivery lifecycle: framing a business problem, documenting requirements, analysing and modelling a process, defining testable user stories, organising delivery work, and reviewing basic API behaviour. The artefacts are intended to support a focused portfolio or interview walkthrough.

## Author

**Sarthak Jaykar** · [GitHub](https://github.com/sarthak-jaykar) · [LinkedIn](https://www.linkedin.com/in/sarthak-jaykar/)
