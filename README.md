# IT Service Request Management — Business Analyst Case Study

## Project Overview

A practical Business Analyst case study demonstrating the end-to-end analysis and documentation of an IT Service Request Management system.

The project follows a realistic BA workflow from identifying the business problem and gathering requirements through process modelling, user stories, Jira implementation, API testing, and solution documentation.

## Business Problem

Organizations often receive IT service requests through inconsistent channels, making it difficult to categorize, prioritize, track, and resolve requests efficiently.

The proposed system provides a structured process for submitting, classifying, prioritizing, tracking, and managing IT service requests.

## Project Objective

The objective was to analyze the business need, define clear requirements, model the current and proposed processes, translate requirements into user stories, implement the work in Jira, and analyze/test the supporting REST APIs.

## BA Approach

**Business Problem → Stakeholder Analysis → Requirements → Process Modelling → User Stories → Jira Implementation → API Analysis & Testing → Proposed Solution**

## Tools Used

* **Confluence** — Business documentation, BRD, requirements, user stories and acceptance criteria
* **Draw.io / BPMN** — AS-IS and TO-BE process modelling
* **Jira** — Epic, user stories, priorities and Kanban workflow
* **Postman** — REST API testing and response validation
* **GitHub** — Project documentation and portfolio evidence

## Key Deliverables

### Requirements Analysis

* Business requirements
* Functional requirements
* Non-functional requirements
* User stories
* Acceptance criteria

### Process Modelling

* AS-IS BPMN process
* TO-BE BPMN process
* Process improvement analysis

### Jira Implementation

* IT Service Request Management Epic
* 9 user stories
* Priorities
* Kanban workflow
* To Do → In Progress → Done workflow

### API Analysis & Testing

The project includes REST API testing using a mock API.

| Method | Operation                | Result      |
| ------ | ------------------------ | ----------- |
| GET    | Retrieve service request | 200 OK      |
| POST   | Create service request   | 201 Created |
| PUT    | Update service request   | 200 OK      |
| DELETE | Delete service request   | 200 OK      |

Postman response validation was also implemented for expected HTTP status codes.

## Repository Structure

```text
IT-Service-Request-Management-BA-Case-Study/
│
├── requirements/
├── process-models/
├── user-stories/
├── jira/
├── api-testing/
├── documentation/
└── notes/
```

## Project Outcome

The project demonstrates the ability to translate a business problem into structured requirements, model business processes, define testable user stories, manage requirements through an Agile/Jira workflow, understand REST API interactions, and maintain professional BA documentation.

## Evidence

The repository contains supporting documentation, BPMN diagrams, user stories, Jira evidence, Postman API testing evidence, and the complete case-study documentation.

## Disclaimer

The API testing component uses a mock REST API for demonstration and learning purposes. The API endpoints represent the type of operations that could support an IT service request system; they are not a production ITSM backend.
