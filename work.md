---
layout: default
title: Work
permalink: /work/
---

<p>
  <a href="/files/resume.pdf" target="_blank">Download Resume</a> &nbsp;·&nbsp;
  <a href="https://github.com/uknth" target="_blank" rel="noopener">GitHub</a>
</p>

---

## Harness — Principal Engineer
**Oct 2025 – Present**

Still relatively new here, but already shipped something I'm pretty happy with.

**Global Notification Service for Feature Flags**

Built an SSE-based notification service that holds ~7 million concurrent connections for the Split.io SDK — delivering real-time feature flag updates with no SDK changes required. Replaced [Ably](https://ably.com) as the vendor, cutting costs by over 60%.

The fun parts: thundering herd on mass reconnect, fan-out delivery guarantees at scale, zero-downtime rollout on a live production system. Stack: Go, NATS, ZeroMQ, inter-service communication over Unix Domain Sockets.

Next up: Agentic AI. 

---

## Unbxd / Netcore — 11 years, 8 months
**Jan 2014 – Oct 2025**

Unbxd is a Search & Discovery platform for e-commerce. I joined as a Software Engineer and left as Director of Engineering and Chief Architect — which in practice meant I wore every hat at least once.

### Principal Architect *(Jan 2022 – Oct 2025)*

**Search Index Improvements**
Improved query performance by 20–30% and cut costs by ~10% by overhauling the search index infrastructure. Introduced a new Query Engine with a custom DSL, custom replica placement and replication, and upgraded the stack to ARM + Apache Solr 9.

**Data Pipeline v2**
Next-gen data pipeline built to address scaling problems the old one simply couldn't handle anymore. Apache Flink for streaming, Apache Druid + Superset for warehousing, CockroachDB for reporting. Custom Flink operator for dynamic on-demand scaling brought operational costs down 30%.

**Catalog Ingestion Pipeline v3**
A highly scalable, event-driven pipeline handling everything from a few thousand to hundreds of millions of catalog products. Built on Argo Workflows on Kubernetes with Spot Instances — cost reduction of 40–60% depending on load.

**Document Store**
High-speed catalog storage for query-time retrieval. Cut serving latency by 20% by trimming data overhead in the stack. Built on PostgreSQL + Aerospike.

**Product Features**
User-level segmentation and merchandising services; traffic classification using Redis + CockroachDB; schema and lifecycle management improvements; analytics reporting on BigQuery.

### Architect *(Jan 2019 – Jan 2022)*

**Inter-Region, Inter-Datacenter Network Topology**
Designed and built the inter-region communication layer for all microservices — event-driven, using NATS for configuration, metadata, and event propagation. Routing is based on index affinity across regions and datacenters.

**AI Data Pipeline**
Custom data lake on S3 + Parquet for training ML models. Kubeflow connectors for easy pipeline access.

**Standardisation of Internal Libraries**
Open-source Go toolkit: [unbxd/go-base](https://github.com/unbxd/go-base). Internal Java starter project and utility library on Quarkus.

### Senior Software Engineer *(Jan 2014 – Jan 2019)*

**Edge Server** — Custom API gateway handling all network operations, observability, and logging.

**Centralised Configuration Management** — Hierarchical rule system across tiers and groups, built on DGraph + NATS.

**Query Pipeline** — Migrated a monolith to microservices. Custom Solr 6.6 fork, custom query parser, similarity class, and search components.

**Other notables** — GitOps-based CD with Flux CD; internal API gateway for inter-team calls; Protobuf + gRPC adoption for inter-service communication (20% latency improvement); contributions across Orchestrators, Query Analysis, Promotions, Analytics Pipeline v1, and more.

---

## Before Unbxd

| Company | Role | Period |
|---|---|---|
| Parablu Inc. | Product Engineer | May 2013 – Jan 2014 |
| Manhattan Associates | Software Engineer | Jul 2012 – May 2013 |
| Tata Consultancy Services | Asst. Software Engineer | Jul 2010 – Jul 2012 |

Full details in the [resume](/files/resume.pdf).

---

## Skills

<div class="skills-list">
  <span>Information Retrieval</span>
  <span>Distributed Systems</span>
  <span>Architecture Design</span>
  <span>Engineering Leadership</span>
  <span>Software As A Service</span>
  <span>Event Driven Design</span>
</div>
