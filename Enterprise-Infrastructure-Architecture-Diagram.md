# Enterprise Infrastructure & Traffic Flow Architecture

High-level system architecture illustrating external client ingress, perimeter security, application tier routing, and asynchronous database replication.

```mermaid
flowchart LR
    User([External / Branch User]) -->|HTTPS / TLS 1.3| WAF[Cloud WAF & Load Balancer]
    WAF --> App[Application Server Cluster]
    App -->|Port 5432 / Internal| DB[(Primary SQL Database)]
    App -->|REST API| Auth[Identity & Access Management]
    DB -.->|Async Replication| Backup[(Disaster Recovery Replica)]
```
