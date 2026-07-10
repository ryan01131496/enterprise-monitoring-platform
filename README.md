# Enterprise Monitoring Platform

A documentation-first portfolio project demonstrating the architecture and design of a centralized monitoring platform built with a Central Server and Agent model.

The platform illustrates how monitoring data is collected from distributed hosts, centralized for management, and presented through a unified dashboard. It focuses on software architecture, engineering design, and platform concepts without exposing proprietary implementation details.

---

## Architecture

The platform consists of a Central Server and multiple monitoring Agents.

* Agents collect metrics and service status from monitored hosts.
* The Central Server receives and manages monitoring data.
* Monitoring information is aggregated into a unified dashboard.
* Push- and pull-based communication support flexible data collection.
* WebSocket enables real-time monitoring updates.

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
| REST APIs                                            |
| Monitoring Services                                  |
| Dashboard Aggregation                                |
| Alert Management                                     |
| Historical Metrics                                   |
| WebSocket Notifications                              |
+------------------------------------------------------+
                           |
                           |
                 +---------+----------+
                 |   Web Dashboard    |
                 +--------------------+
```

---

## Engineering Highlights

* Central Server and Agent architecture
* Push/Pull hybrid communication
* Heartbeat-based monitoring
* Modular platform design
* Dashboard aggregation
* WebSocket-based real-time updates
* Extensible monitoring architecture

---

## Technology Stack

**Backend**

Java · Spring Boot · Spring Security · RESTful API · WebSocket

**Frontend**

Vue 3 · TypeScript · Pinia · Chart.js · ECharts

**Database**

MySQL

**Architecture**

Central Server · Agent Architecture · Push/Pull Hybrid · Modular Architecture

---

## Repository Scope

This repository focuses on software engineering concepts, architecture, and design decisions.

It does not include proprietary source code, production configurations, client information, internal documentation, or other confidential assets.
