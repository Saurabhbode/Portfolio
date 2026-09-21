# SpineGen-i

For the web design, I would not display all of this as one continuous wall of text. The strongest hierarchy would be: hero/project identity → tech-stack strip → three impact metrics → “My Contribution” ownership section → product capabilities → architecture → technical highlights. In particular, put the tech stack immediately under the project title as prominent chips/badges, and make “Sole Full-Stack Developer — End-to-End Ownership” one of the largest headings on the page.

Your 75%, 85%, and ~15% figures should also be large metric cards near the top. That makes the page communicate impact + ownership + technical depth within the first screen or two, rather than making a recruiter read the entire case study to discover those points.

### Enterprise Operations & Revenue-Cycle Management Platform

**Role:** Sole Full-Stack Developer
**Status:** Production
**Ownership:** End-to-End Product Engineering

**Core Tech Stack:**
**React · JavaScript · Java 17 · Spring Boot · Spring Security · MySQL · Docker · AWS · GitHub Actions**

---

## Project Overview

**SpineGen-i** is a production-grade enterprise operations and Revenue Cycle Management (RCM) platform designed to consolidate complex operational workflows into a single, secure application.

The platform replaced workflows previously distributed across multiple third-party applications and provides operations, finance, management, and administrative teams with one centralized system for managing:

**Users · Teams · Projects · Work Allocation · Claims · AR Aging · Initial Coding · Timesheets · Invoices · Productivity · Reporting · Documents**

I developed SpineGen-i as the **sole Full-Stack Developer**, taking ownership of the complete product lifecycle—from understanding business requirements and designing the system architecture to frontend and backend development, database engineering, testing, cloud deployment, CI/CD, production support, and continuous enhancement.

---

# Business Impact

### 75% Faster User Allocation

Redesigned allocation and assignment workflows using project-based visibility, bulk operations, role-aware access, and streamlined user management.

The resulting workflow reduced allocation processing time by approximately **75%**.

### 85% Reduction in Operating Costs

Consolidated functionality previously handled through multiple third-party products into a single internally owned platform, reducing software and operational expenditure by approximately **85%**.

### Infrastructure at ~15% of Previous Cost

Designed and deployed a containerized AWS infrastructure capable of supporting the application at approximately **15% of the previous external-platform cost**.

### One Centralized Operational Platform

Unified operational data, workflows, reporting, user management, finance processes, and productivity tracking within one application, reducing context switching and manual coordination between systems.

---

# My Contribution

## Sole Full-Stack Developer — End-to-End Ownership

I was responsible for the **complete engineering lifecycle of SpineGen-i**, covering product design, application development, infrastructure, testing, deployment, and production support.

### Product & Solution Architecture

* Translated operational and business requirements into technical workflows and scalable application architecture.
* Designed frontend, backend, database, security, integration, and deployment architecture.
* Converted complex RCM and operational processes into structured digital workflows.
* Designed reusable modules capable of supporting multiple departments, projects, teams, and user roles.

### Frontend Engineering

Built the complete frontend as a **React single-page application using Vite**.

Implemented reusable components and service layers to separate presentation, API communication, authentication, and business workflows.

Developed data-intensive operational interfaces using **AG Grid**, including:

* Advanced filtering and sorting
* Pagination
* Inline workflow actions
* Bulk operations
* Configurable columns
* Persistent user grid preferences
* High-volume operational datasets

Implemented interactive reporting and productivity visualizations using **ECharts**.

### Backend Engineering

Designed and developed the backend using **Java 17 and Spring Boot** following a layered architecture:

**Controller → Service → Repository → MySQL**

The backend includes:

* Secure REST APIs
* Business-rule processing
* Workflow orchestration
* Allocation logic
* Reporting services
* Spreadsheet reconciliation
* Validation
* Authentication and authorization
* Scheduled processing
* File and document management

Used **Spring Data JPA and Hibernate** for persistence while maintaining DTO-based separation between API contracts and database entities.

### Database Engineering

Designed the relational **MySQL** data model supporting users, organizational hierarchies, projects, tasks, claims, invoices, timesheets, productivity, reporting, configuration, comments, attachments, and audit history.

Implemented:

* Relational schema design
* Foreign-key relationships
* Database indexing
* Query optimization
* Version-controlled schema migrations
* Production database upgrades
* Data validation and integrity controls

### Security Engineering

Implemented a layered application security model using **Spring Security**.

Security capabilities include:

* Secure authentication
* JWT/session controls
* Password hashing
* Role-Based Access Control (RBAC)
* Project-scoped authorization
* Fine-grained navigation permissions
* Controlled session expiration
* Server-side validation
* Protected REST endpoints
* Password-reset workflows
* Email verification
* Expiring reset tokens
* CAPTCHA protection
* Audit logging

The authorization model ensures users can access only the projects, navigation areas, and operational data permitted by their assigned role and project membership.

### DevOps & Cloud Deployment

Designed containerized environments using **Docker and Docker Compose** for consistent development, staging, and production deployments.

Built an automated **GitHub Actions CI/CD pipeline** covering application validation, builds, container-image creation, publishing, and production deployment.

Managed the production environment using:

**AWS EC2 · AWS S3 · Docker · Nginx · HTTPS · Let's Encrypt**

Environment-specific configuration and secrets are maintained outside source control to improve deployment security.

### Testing & Quality Engineering

Implemented automated and manual testing across the application lifecycle.

Testing includes:

* Unit testing
* Integration testing
* Functional testing
* API testing
* End-to-end testing
* Browser automation
* Regression testing
* Critical workflow validation

Technologies include **Vitest, React Testing Library, Spring Boot Test, Mockito, and Playwright**.

Automated browser tests cover critical user journeys, while dedicated testing was implemented for data-intensive dashboards, timesheets, authentication, and operational workflows.

---

# Key Product Capabilities

## Operations & Work Allocation

Built centralized operational workflows supporting project-, customer-, department-, team-, and user-level work management.

Key capabilities include:

* Intelligent user allocation
* Project-based user visibility
* Team hierarchy management
* Role-aware assignments
* Bulk claim operations
* Assignment history
* Comment history
* Workflow traceability
* Configurable work statuses
* Work-source management
* Action categories
* Denial and rejection configuration
* Revenue-status tracking

These capabilities allow high-volume operational teams to assign, track, update, and audit work efficiently.

---

## Revenue-Cycle Management

Developed specialized workflows for Revenue Cycle Management operations.

### AR Aging

Built AR-aging management with:

* Claim-level tracking
* Assignment workflows
* Status management
* Aging-related processing
* Reconciliation
* Comments and history
* Attachments
* Automated scheduled processing

### Initial Coding

Developed configurable initial-coding workflows supporting:

* Work routing
* Lookup configuration
* Turnaround-time tracking
* Assignment
* Attachments
* Operational status management

### Finance & Invoicing

Implemented finance-oriented capabilities including:

* Invoice generation
* Invoice history
* Printable invoice views
* Cash-log management
* Financial workflow tracking
* Operational reconciliation

---

# Productivity & Analytics

Built productivity and performance-management capabilities that provide management with visibility into operational output.

Features include:

* Employee timesheets
* Project-level time tracking
* Task-level time tracking
* Weekly timesheet copy
* Reporting hierarchies
* Daily productivity reporting
* Hourly productivity analysis
* Production-analysis dashboards
* Interactive charts
* Data-grid reporting
* Date-based operational analysis

User-specific dashboard and grid preferences are persisted to provide a consistent personalized experience.

---

# Spreadsheet Automation

One of the platform's core engineering capabilities is its high-volume spreadsheet processing and reconciliation engine.

Built import pipelines supporting:

**Excel · XLSX · CSV**

Using **Apache POI** and application-level validation, the platform performs:

**Upload → Header Mapping → Validation → Duplicate Detection → Reconciliation → Processing → Summary Generation**

The processing engine handles:

* Invalid rows
* Missing fields
* Duplicate records
* Re-uploaded records
* Existing claim reconciliation
* Status updates
* Partial-success uploads
* Failed-record reporting

Users receive downloadable processing summaries identifying **accepted, skipped, duplicate, and failed records**, significantly improving transparency during large operational uploads.

---

# File & Document Management

Implemented secure document and spreadsheet attachment workflows throughout the platform.

Production files are integrated with **AWS S3**, allowing application data and file storage to remain independently scalable.

The platform supports controlled file uploads, downloads, attachments, and workflow-specific document management.

---

# Technical Architecture

### Frontend

**React · JavaScript · Vite · React Router · Axios · AG Grid · ECharts · XLSX**

React provides the application shell and reusable UI architecture, while AG Grid powers data-intensive operational interfaces and ECharts provides analytical visualization.

### Backend

**Java 17 · Spring Boot · Spring Security · Spring Data JPA · Hibernate · Maven**

Spring Boot provides REST services, business workflows, security, validation, reporting, scheduled processing, and integration services.

### Database

**MySQL · SQL · Versioned Database Migrations**

The relational database architecture supports transactional operational data, reporting, configuration, auditability, and workflow history.

### Security

**Spring Security · JWT · RBAC · Session Management · Project-Scoped Authorization · Server-Side Validation**

Security controls operate across API, navigation, project, role, and data-access levels.

### Cloud & DevOps

**AWS EC2 · AWS S3 · Docker · Docker Compose · Nginx · GitHub Actions · Let's Encrypt**

Containerization and CI/CD provide repeatable builds and consistent deployments across development, staging, and production environments.

### Testing

**Vitest · React Testing Library · Spring Boot Test · Mockito · Playwright**

Automated testing covers frontend components, backend business logic, integration points, and critical end-to-end workflows.

### Integrations & Processing

**Apache POI · iText PDF · Spring Mail**

Used for spreadsheet automation, document/PDF generation, and application email workflows.

---

# Technical Highlights

* Architected and developed a **production enterprise platform from the ground up as the sole developer**.
* Designed REST APIs covering users, roles, teams, projects, tasks, claims, invoices, timesheets, dashboards, sheets, comments, attachments, and reporting.
* Implemented **project-scoped authorization** to prevent unauthorized cross-project data access.
* Built a robust **spreadsheet reconciliation engine** capable of processing invalid rows, duplicates, re-uploads, updates, and partial successes.
* Implemented scheduled backend processing for time-sensitive **AR-aging workflows**.
* Designed database indexes and version-controlled migrations to support growing operational datasets.
* Created separate **local, staging, and production Docker environments** for reproducible releases.
* Built an automated **CI/CD pipeline using GitHub Actions**.
* Deployed and maintained the application on **AWS EC2 with Nginx and HTTPS**.
* Integrated **AWS S3** for production document storage.
* Implemented automated browser testing for business-critical workflows.
* Continued ownership after production launch through performance optimization, security hardening, database migrations, bug resolution, and feature development.

---

# Technology Stack

### Frontend

**React · JavaScript · Vite · React Router · Axios · AG Grid · ECharts · XLSX**

### Backend

**Java 17 · Spring Boot · Spring Security · Spring Data JPA · Hibernate · Maven**

### Database

**MySQL · SQL · Database Migrations**

### Security

**JWT · Session Management · RBAC · Project-Level Authorization · Navigation Permissions · Server-Side Validation**

### Cloud & DevOps

**AWS EC2 · AWS S3 · Docker · Docker Compose · Nginx · GitHub Actions · HTTPS · Let's Encrypt**

### Testing

**Vitest · React Testing Library · Spring Boot Test · Mockito · Playwright**

### Integrations

**Apache POI · iText PDF · Spring Mail**

---

# Project at a Glance

**Role:** Sole Full-Stack Developer
**Environment:** Production
**Architecture:** React SPA + Spring Boot REST API + MySQL
**Deployment:** Docker + AWS EC2 + Nginx
**Storage:** AWS S3
**CI/CD:** GitHub Actions
**Security:** Spring Security + RBAC + Project-Scoped Authorization
**Testing:** Unit + Integration + E2E Automation

**75%** reduction in allocation processing time
**85%** reduction in operating costs
**~15%** of previous infrastructure/platform cost

---

## Portfolio Summary

Built **SpineGen-i** from the ground up as the **sole Full-Stack Developer**, delivering a production-grade enterprise operations and Revenue Cycle Management platform that replaced multiple third-party systems with a single internally owned solution.

I owned the complete engineering lifecycle—including **solution architecture, React frontend development, Spring Boot APIs, MySQL database design, application security, RBAC, spreadsheet automation, AWS infrastructure, Docker containerization, CI/CD, automated testing, deployment, and ongoing production development**.

The platform delivered measurable business impact, including a **75% reduction in user-allocation processing time** and an **85% reduction in operating costs**, while operating at approximately **15% of the previous platform and infrastructure cost**.
