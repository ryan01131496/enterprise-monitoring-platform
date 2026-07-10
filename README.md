# Enterprise Monitoring Platform

A generalized architecture case study of a centralized monitoring platform built with a Central Server and Agent model.

This repository presents architectural concepts, engineering decisions, and platform design approaches for centralized monitoring systems. All technical content has been generalized from professional engineering experience and intentionally excludes proprietary implementation details.

---

## Architecture

The platform follows a modular architecture centered around a Central Server and multiple monitoring Agents.

Monitoring Agents collect metrics and service health information from distributed hosts, while the Central Server aggregates monitoring data, coordinates monitoring services, and provides a unified operational view.

The architecture combines push- and pull-based communication to support flexible monitoring scenarios and uses WebSocket for real-time status updates.

```text
                +----------------------+
                | Monitoring Agent(s)  |
                |----------------------|
                | Metrics Collection   |
                | Heartbeat            |
                | Service Check        |
                +----------+-----------+
                           |
                     Push / Pull
                           |
+------------------------------------------------------+
|                   Central Server                     |
|------------------------------------------------------|
| RESTful Services                                     |
| Monitoring Services                                  |
| Dashboard Aggregation                                |
| Alert Management                                     |
| Historical Metrics                                   |
| Real-time Notifications                              |
+------------------------------------------------------+
                           |
                           |
                 +---------+----------+
                 |   Web Dashboard    |
                 +--------------------+
```

---

## Engineering Highlights

* Central Server and Agent Architecture
* Push/Pull Hybrid Communication
* Heartbeat Monitoring
* Metrics Collection
* Service Health Monitoring
* Dashboard Aggregation
* Real-time Communication
* Modular Platform Design
* Extensible Monitoring Architecture

---

## Technology Stack

**Backend**

Java · Spring Boot · Spring Security · RESTful API · WebSocket

**Frontend**

Vue 3 · TypeScript · Pinia · Chart.js · ECharts

**Database**

MySQL

**Architecture**

Central Server Architecture · Agent-based Architecture · Push/Pull Hybrid Architecture · Modular Architecture · Dashboard Aggregation

---

## Repository Scope

This repository is a generalized architecture case study intended to demonstrate software architecture, engineering design, and platform-oriented thinking.

It does not represent a production system or the complete implementation of any organization.

To protect confidentiality, this repository intentionally excludes proprietary source code, internal identifiers, client information, business rules, production configurations, API specifications, database schemas, deployment details, logs, screenshots, credentials, and other confidential assets.
