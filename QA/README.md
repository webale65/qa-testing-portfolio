# QA Testing Portfolio – RiderFit Project

This repository contains the **Quality Assurance documentation and deliverables** produced during the development of the **RiderFit (FitBot)** project.

The project was developed as part of the **No Country professional simulation**, where the team worked collaboratively using **Agile methodology (Scrum)** and a **Gitflow-based workflow** in GitHub.

---

## RiderFit – Project Context

**RiderFit** is an intelligent assistant integrated into an e-commerce platform designed to help riders select the correct equipment size by analyzing both **rider measurements and horse measurements**.

Project repository:
https://github.com/No-Country-simulation/S02-26-Equipo12-WebAppDevelopment

---

## QA Role and Responsibilities

During the project I participated as a **Quality Assurance Tester**, contributing to the validation of system functionality and identifying potential defects during the development lifecycle.

Main QA responsibilities included:

* Functional testing of system features
* API testing using **Swagger** and **Postman**
* Frontend–Backend integration validation
* Backend environment validation
* Database validation using **PostgreSQL**
* Pull Request technical reviews
* Bug detection and documentation
* QA documentation and test evidence management

---

## QA Contributions in the RiderFit Project

### Example QA Finding — RiderForm Measurement Duplication

RiderForm Measurement Duplication

Severity: High

Description:
Updating rider measurements using the PUT operation may generate duplicated records when previous measurements are not validated.

Recommendation:
Validate the existence of previous measurements before inserting a new record in the database.

Examples of QA contributions within the project repository:

**QA Issues created**

Issue #38 – Backend environment validation and database synchronization
https://github.com/No-Country-simulation/S02-26-Equipo12-WebAppDevelopment/issues/38
Issue #17 – Global state architecture validation (Zustand)
https://github.com/No-Country-simulation/S02-26-Equipo12-WebAppDevelopment/issues/17

**Pull Request Reviews**

PR #45 – Login implementation  
https://github.com/No-Country-simulation/S02-26-Equipo12-WebAppDevelopment/pull/45

PR #56 – RiderForm validation  
https://github.com/No-Country-simulation/S02-26-Equipo12-WebAppDevelopment/pull/56

PR #60 – HorseForm measurements  
https://github.com/No-Country-simulation/S02-26-Equipo12-WebAppDevelopment/pull/60

These contributions helped identify architectural inconsistencies, potential defects, and integration issues during development.

Additional QA evidence includes API validation, database consistency checks, UUID/input validation analysis, re-testing activities, and private route protection testing documented in project issues.

## Pull Request Reviews

During the RiderFit project I also participated in the technical review of Pull Requests to validate integration and ensure compliance with QA guidelines.

Example PR reviews:

PR #56 – RiderForm validation  
Result: REQUEST CHANGES

Findings:

- Inconsistency between frontend measurementTypeId values and backend database records.
- measurement types generated dynamically in database seeds while frontend uses hardcoded UUIDs.
- API returns 404 – MeasurementType not found.

Impact:

Frontend–Backend integration cannot be validated until measurement types are aligned.

PR #45 – Login implementation  
Result: BLOCKED

Findings:

- Merge conflicts detected in Login component files.
- Entry point inconsistency in index.astro where LoginPage and Fitbot were rendered simultaneously.

Impact:

Login flow cannot be validated until merge conflicts are resolved and navigation logic is clarified.

---

## Tools and Technologies

**Testing**

* Manual Testing
* API Testing

**Tools**

* Postman
* Swagger
* GitHub
* Gitflow

**Database**

* PostgreSQL

**Methodology**

* Agile
* Scrum
* Sprint-based workflow

---

## QA Documentation Included

This repository contains the following QA deliverables:

**QA Final Report**
Comprehensive report describing the QA strategy, testing process, and findings.

**Bug Reports**
Documented defects identified during testing, including severity classification and reproduction steps.

**Test Cases**
Structured functional test scenarios designed to validate key system behaviors.

**Traceability Matrix**
Mapping between system requirements and corresponding test cases to ensure test coverage.

---

## Purpose of this Repository

This repository serves as a **QA portfolio**, providing evidence of the testing process applied during the RiderFit project and demonstrating practical experience in:

* Software quality assurance
* defect detection and documentation
* API validation
* collaborative development workflows

The documentation reflects how QA contributes to improving system reliability and software quality within an Agile development environment by applying structured testing, defect identification, and technical validation of application components.

