---
title: Work Experience
layout: page
permalink: '/experience/'
---

## [Meta Platforms](#meta)

### Production Engineer &mdash; January 2019 - Present

#### Release Integrity Lead
- Reduced p90 production binary age from 70 days to 5 days while maintaining perfect production reliability.
- Prevented previously undetectable silent data corruption by automatically blocking a regression release.
- Accelerated release validation signals and improved cluster efficiency by designing and building Fulcrum, a solver layer for SEF that dynamically shifted 2% of traffic from overutilized to underutilized clusters.
- Scaled deferred correctness validations (checksum, partition latency, delta merge) across 4 products.
- Designed and implemented SEF, a scenario framework enabling engineers to rapidly and easily onboard new validation scenarios.

#### Global Tetris and Disaster Recovery Lead
- Eliminated 240 PB of excess backfill by collaborating with the replication team.
- Reduced end-to-end failover time from 80 minutes to 5 minutes using a modernized workflow implementation.
- Increased DR storm cadence from quarterly to weekly by leveraging automated workflows.
- Fully automated disaster workflow by developing and deploying a location-availability aware regional PinStore using Manifold blob storage.
- Prevented a major outage due to DR storms by leading a month-long sprint to eliminate 99% of work for Multi-Region namespaces.
- Reduced SLO misses from DR drills to 0 (from 4 per half) and reduced unneeded work for Multi-Region drain/undrain by 53-78%.
- Designed and built a symmetric API for DR execution, simplifying execution and improving reliability of key tooling; landed a Multi-Region Aware Analysis Pipeline for one-command DR execution.
- Validated capacity requirements for 10 batches of initial migrations, facilitating the split of the largest ads namespace (critical to revenue) across 3 datacenter regions.
- Corrected cost forecasting for 15-minute partitions, resulting in 75% more accurate cost estimates.
- Landed DR capacity sharing model for DB Ingestion, allowing net 0 DR capacity budget used for Sesame DR.
- Added monitoring for paused jobs during failover and landed readiness monitoring for Synapse to detect failures and prevent recovery delays.
- Organized quarterly internal DR Dress Rehearsals, stress-testing tooling and documentation.

#### Capacity Roadmap Owner
- Saved $20M annually in server capex and reduced regional capacity variance by 5% by designing and building bulk cluster automation tooling to facilitate migration to shared infrastructure.
- Reduced over-ordering by 50+ racks and cut quarterly dev effort from 2-3 days to ~2 hours by driving a multi-half effort to integrate FBETL with Warehouse capacity planner.
- Completed Synapse throughput analysis, enabling more accurate sizing of Synapse cluster.
- Created foundational pillar and 3-year capacity vision, driving roadmap planning across multiple halves.
- Built distributed scheduler exclusion lock, preventing control plane duplication and reliability risks.
- Influenced DB ingestion onboarding onto capacity planning tooling using a pseudo-namespace proposal.

#### Better Engineering Lead
- Contributed to a >85% task closure rate within 30 days org-wide by forming and leading a teamwide SEV committee, reducing the team's followup backlog age from an average of 150 days to 20 days.
- Saved hundreds of engineering hours by reducing primary CLI cold start times by 60-70% via reduced schema fetching and module loading overhead.
- Consistently cut build/test flakiness by 30-40% every 6 months, accelerating development on an ongoing basis.
- Built and rolled out OS stats-based health check framework to DIMS (global ingestion control plane), preventing overloaded hosts from impacting service reliability.
- Reduced p99 latency by 50% on DIMS, and automated heap dump collection on FULLGC events.
- Eliminated a major cause of oncall pain by reducing push failures from 70% to 5% and reduced build failures by 30% by fixing a Python capacity library concurrency issue.
- Built cross-pod Service Excellence goal-tracking dashboard and a team process for driving weekly root-cause analysis to prioritize oncall improvements.
- Removed a consistent pain point in C++ development by correcting ephemeral build lifetime and extending test cluster lifetimes.
- Drove C++ from a production readiness perspective, launching with instance health checks, capacity attribution, continuous push, and integration testing.

> "Tyler played a critical role in multiple SEV mitigations regardless of whether he was oncall. His dedication, prompt response, and generosity to offer help are deeply valued." -- Peer feedback

#### Data Infra SEV Review Core Team & Safety Lockdown
- Planned and moderated weekly incident management reviews on an org-wide level, collecting impact metrics and proposing improvements across diverse services.
- Led safe config rollout work for Scribe Ingestion services, resulting in ~156 diffs canaried per day.
- Led end-of-half release improvement fixathon, using a common health check framework to reduce release validation time by ~2 hours per check.

#### Technical Mentorship
- Unblocked 1MW of efficiency work through load-test automation and autoscaling.
- Mentored three junior engineers on career growth and technical blockers, and coached four interns to successful projects/return offers.

## [Buddy Platform](#buddy-platform)

### Engineering Lead &mdash; February 2018 - December 2018
- Introduced REJI (Rapid Engineer Joy Index), a 0-5 quick assessment of three dimensions of job satisfaction during standup.
- Led design, development, and deployment of Feeds, a portfolio concept to allow grouping and basic aggregation of energy data to support three-phase circuit monitoring using Elasticsearch.
- Designed and implemented a graph database to implement portfolio service to flexibly handle arbitrary entity depth, ACL and role-based security with inheritance.
- Designed ingestion pipeline composed of four independent dropwizard microservices, deployed on Marathon/Mesos and communicating using Azure Event Hubs and Avro serialization.

### Senior Software Engineer &mdash; Jan 2014 - Feb 2018
- Refactored time series database architecture into polymorphic implementations.
- Architected and managed pluggable data processing pipeline based on the Apache Spark stack.
- Designed and implemented CoreOS system architecture using concepts from immutable infrastructure to deliver rapid deployments and rollbacks and reduce Azure spend 30%.
- Designed and implemented DataSource/DataSink pipeline for creating composable data transformation objects that can run across computing platforms.
- Migrated MongoDB cluster to LVM/LUKS/RAID-10 configuration backed by Azure premium blob storage; changes merged into upstream Chef 12.
- Redesigned telemetry architecture using an asynchronous stream architecture, allowing telemetry manipulation, filtering, and recording to happen in parallel.
- Architected and implemented extensible state machine model of push notification registration and delivery transparently spanning Azure Notification Hubs and Amazon SNS.

## [Amazon.com](#amazoncom)
### Web Development Engineer, Wireless CX Team &mdash; Sept 2011 – Dec 2014
- Reduced perceived latency of UI actions by batching together AJAX requests and sending them invisibly while performing intermediate price computations on the browser.
- Redesigned wireless plans and options page to use reusable JSP taglib components and an extensible decorator pattern.
- Converted all PUC pages to DataProvider architecture, decoupling UI from dependent services by injecting static data through Spring.
- Managed migration from a BDB artifact for localized strings to Localization Metadata Service, reducing the time needed to push string revisions from 2 weeks to 15 minutes.
- Increased code coverage of key library packages (AlohaAppsLib and AlohaPUCLib) by 20% and 15% respectively.
- Migrated amazonwireless.com to amazon.com, creating a unified shopping experience for contract phones on the retail website.
- Implemented configurable zip code driven tax display system to inform customers of the tax policies of certain states.

## [Health Plan Services](#health-plan-services)
### Senior Web Developer &mdash; Sept 2009 – Sept 2011
- Led architecture, design, and development of initial implementation of a mobile quoting application for iPad and iPhone using XCode3 and Cocoa Touch.
- Drove an organizational push for test-driven development and continuous integration using PHPUnit and CruiseControl.
- Together with two other senior developers, designed and architected a modular and extensible enterprise enrollment system used by Cigna, Beazley, and Freelancers Union.
- Led architecture, design, implementation, and testing of an event-driven workflow engine (SINEWE) for tracking and restoring user state across web interfaces based on principles observed in Spring Web Flow and BPEL.
- Led design and development of a database configurable PHP controller class to produce a daily feed of TIFF images retrieved from an internal Stellent server for Humana.

## [Verizon Business](#verizon-business)
### Software Systems Engineer IV &mdash; Jan 2009 - Sept 2009
- Prepared the IPM suite for enterprise deployment by implementing input validation classes and query parameterization using PHP and MySQL on an existing code base of more than 600,000 lines supporting 13,000 active users.
- Designed and implemented session-based metadata caching layer to store template specific data on web servers, providing speed improvements of 10-15 seconds.
- Employed document revisioning classes to create a living Business Requirement document providing document workflow and traceability.
