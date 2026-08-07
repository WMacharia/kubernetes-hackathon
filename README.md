# Widgetario Kubernetes Hackathon

## Group Members

- **Macharia Grace Wairimu 165899**
- **Deborah Rehana Kerubo 168656**
- **Billiart .B. Mwangi 164099**
- **Elijah Njugi Muiru 146412**

---

# Project Overview

This repository contains our solution to the **Widgetario Kubernetes Hackathon**, a hands-on DevOps and Cloud Computing exercise focused on deploying, managing, observing, and automating a microservices application using Kubernetes.

The hackathon progressively introduces industry-standard Kubernetes concepts, requiring participants to transform a collection of containerized services into a production-ready cloud-native application.

Rather than solving one isolated problem, the hackathon builds a complete deployment pipeline, beginning with basic Kubernetes workloads and ending with observability and Continuous Integration/Continuous Deployment (CI/CD).

---

# Learning Objectives

Throughout this project we gained practical experience in:

- Kubernetes architecture
- Container orchestration
- Microservices deployment
- High availability and fault tolerance
- Service discovery
- Stateful applications
- Kubernetes networking
- Ingress configuration
- Persistent storage
- Monitoring using Prometheus
- Visualization using Grafana
- Centralized logging using the EFK Stack
- Helm package management
- Continuous Integration and Continuous Deployment principles

---

# Technologies Used

- Kubernetes
- Docker
- Kind (Kubernetes in Docker)
- kubectl
- NGINX Ingress Controller
- PostgreSQL
- Spring Boot
- Go
- Prometheus
- Grafana
- Elasticsearch
- Fluent Bit
- Kibana
- Helm
- Jenkins

---

# Application Architecture

The Widgetario application consists of four primary microservices:

| Component | Purpose |
|-----------|----------|
| Web | Frontend user interface |
| Products API | Product catalogue service |
| Stock API | Inventory management service |
| Products Database | PostgreSQL database |

Each service is deployed independently, allowing Kubernetes to manage scaling, recovery and communication between components.

---

# Hackathon Progression

The hackathon is divided into several incremental stages. Each stage introduces new Kubernetes concepts while building upon previous work.

## Part 1 – Kubernetes Fundamentals

Objectives:

- Deploy applications using Deployments
- Deploy PostgreSQL
- Create ClusterIP Services
- Understand Pods and ReplicaSets
- Verify application communication

Key concepts learned:

- Deployments
- ReplicaSets
- Pods
- Labels
- Selectors
- Services
- Cluster networking

---

## Part 2 – Scaling

Objectives:

- Scale application replicas
- Load balancing across Pods
- Validate Kubernetes self-healing

Key concepts learned:

- Horizontal scaling
- Fault tolerance
- Replica management
- High availability

---

## Part 3 – Stateful Applications

Objectives:

- Deploy PostgreSQL as a StatefulSet
- Configure persistent storage

Key concepts learned:

- StatefulSets
- Persistent Volumes
- Persistent Volume Claims
- Stable networking
- Storage management

---

## Part 4 – Networking

Objectives:

- Configure Ingress
- Deploy NGINX Ingress Controller
- Configure host routing

Key concepts learned:

- Ingress
- Reverse proxy
- HTTP routing
- Load balancing
- DNS host mapping

---

## Part 5 – Application Configuration

Objectives:

- Configure Secrets
- Configure ConfigMaps
- Mount configuration into containers

Key concepts learned:

- Secret management
- Configuration management
- Environment configuration

---

## Part 6 – Observability

Objectives:

Deploy monitoring and centralized logging.

### Monitoring Stack

- Prometheus
- Grafana

Implemented:

- Prometheus metrics scraping
- Application metrics
- Grafana dashboard import
- Performance visualization

Metrics collected include:

- CPU usage
- Memory usage
- Request rate
- JVM metrics
- Application health

### Logging Stack

- Elasticsearch
- Fluent Bit
- Kibana

Implemented:

- Centralized log aggregation
- Sidecar logging for the web application
- Dashboard visualization
- Log searching

This stage demonstrated how production Kubernetes clusters monitor both application health and runtime behaviour.

---

## Part 7 – Continuous Integration / Continuous Deployment

Objectives:

- Package the application using Helm
- Deploy multiple releases
- Build CI/CD pipeline
- Automate deployments

Technologies introduced:

- Helm Charts
- Jenkins
- Docker Registry
- Automated deployments

Although the complete CI/CD pipeline was beyond the initial deployment objectives, this stage illustrates how Kubernetes integrates with modern DevOps workflows.

---

# Repository Structure

```
hackathon/
│
├── files/
│
├── project/
│
├── solution-part-1/
├── solution-part-2/
├── solution-part-3/
├── solution-part-4/
├── solution-part-5/
├── solution-part-6/
├── solution-part-7/
│
└── README.md
```

---

# Purpose of Each Folder

## files/

Contains supporting resources used throughout the hackathon, including:

- Grafana dashboards
- Kibana dashboards
- Helm configuration files
- Supporting assets

These resources are imported into monitoring and visualization tools during deployment.

---

## project/

Contains the application source code and CI/CD configuration including:

- Jenkins pipeline
- Build configuration
- Application source

This folder represents the production application being deployed.

---

## solution-part-1 → solution-part-7/

Each solution folder represents the completed configuration for a specific stage of the hackathon.

These folders are intentionally independent.

Each stage builds upon previous concepts while introducing additional Kubernetes functionality.

Examples include:

- Deployments
- Services
- StatefulSets
- Ingress
- Monitoring
- Logging
- Helm packaging

They also serve as reference implementations whenever troubleshooting or validating configurations.

---

# Skills Demonstrated

By completing this project we demonstrated competency in:

- Kubernetes resource management
- YAML configuration
- Docker image deployment
- Microservices orchestration
- Cluster networking
- Service discovery
- High availability
- Scaling applications
- Production monitoring
- Centralized logging
- Cloud-native architecture
- Infrastructure troubleshooting

---

# Challenges Encountered

During the implementation several practical challenges were encountered, including:

- Kubernetes Service configuration
- Port forwarding
- NodePort access
- Ingress controller deployment
- Prometheus target configuration
- Grafana dashboard setup
- Kibana dashboard configuration
- Fluent Bit log forwarding
- Resource allocation and memory constraints
- Pod restart troubleshooting
- CrashLoopBackOff diagnosis
- GitHub Push Protection
- Image registry configuration

Resolving these issues provided valuable experience with real-world Kubernetes debugging and operational workflows.

---

# Key Takeaways

This hackathon reinforced that deploying applications to Kubernetes extends beyond simply running containers.

A production-ready deployment requires:

- Reliable networking
- Persistent storage
- Configuration management
- Secrets management
- Monitoring
- Centralized logging
- Fault tolerance
- Automated deployment pipelines

The project demonstrates how modern cloud-native systems combine these technologies to create scalable, observable, and resilient applications.
