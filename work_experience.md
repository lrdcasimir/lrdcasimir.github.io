---
title: Work Experience
layout: page
permalink: '/experience/'
---

## [Meta Platforms](#meta)

### Production Engineer &mdash; January 2019 - Present

- **Global Tetris and Disaster Recovery Lead**
 - Landed Multi-Region Aware Analysis Pipeline, allowing for one-command DR execution 
  of Multi-Region namespace failover and capacity automation
 - Reduced SLO misses due to DR drills to 0 from 4 per half
 - 53% and 78% reduction in unneeded work for Multi-Region drain and undrain
 - Proposed, designed, implemented and built a symmetric API for DR execution,
   simplifying execution and improving reliability of key tooling
 - Added monitoring for paused jobs during failover to detect failures before developing into SEVs
 - Corrected cost forecasting for 15 minute partitions, resulting in more accurate cost estimates by 75%
 - Landed DR capacity sharing model for DB Ingestion, allowing net 0 DR capacity budget used for Sesame DR
 - Organized quarterly internal DR Dress Rehearsals, stress testing tooling and documentation and following up on gaps
 - Landed readiness monitoring for Synapse to avoid recovery delays due to destructive resize operations in Synapse clusters
 - Led a month-long sprint to eliminate 99% of work for Multi-Region namespaces, prevening a major outage due to DR storms
 - Validated capacity requirements for 10 batches of initial migrations, faciliting the split of the largest ads namespace,
   critical to revenue, across 3 datacenter regions
- **Capacity Roadmap Owner**
 - Completed Synapse throughput analysis, enabling more accurate sizing of Synapse cluster
 - Created foundational pillar and 3 year capacity vision, driving roadmap planning across multiple halves
 - Guided design of quota enforcement across peers and stakeholders
 - Influenced DB ingestion onboarding onto capacity planning tooling using a psuedo-namespace proposal
 - Drove multi-half effort to integrate FBETL with Warehouse capacity planner, resulting in reduced over-ordering by 50+ racks, reduced
   quarterly dev effort from 2-3 days to ~2 hours
 - Designed and built bulk cluster automation tooling, facilitating migration to fully shared infrastructure, resulting in 5% reduced 
   regional capacity variance in production and saving $20M annually in server capex
 - Built distributed scheduler exclusion lock, preventing control plane duplication and reliability risks
- **Better Engineering Lead**
 - Build cross pod Service Excellence goal-tracking dashboard to track oncall load and progress toward service maturity levels over time
 - Build team process for oncall improvement by tracking top oncall pain points and driving weekly root-cause analysis to
   drive oncall improvement prioritization
 - Refactored cluster automation to more flexibly add product-specfic components without increased complexity
 - Reduced primary cli cold start times by 60-70% by reducing schema fetching and module loading overhead, saving 10s of hours of
   developer time spent waiting on tooling
 - Consistently reduced build/test flakiness by 30-40% every 6 months, cutting build times and accelerating development
   on an ongoing basis
 - Formed and led a teamwide SEV committee to review and prioritize followups from incidents, reducing the team's 
   followup backlog age from an average of 150 days to 20 days and improving task completon behavior team-wide from 1 critical followup per week to 6.
   Org-wide this contributed to a >85% task closure rate within 30 days for the most critical followps.
 - Created Service Maturity Gap analysis and proposed milesone delivery schedule
 - Built and rolled out OS stats-based health check framework to DIMS, the global ingestion control plane,
   preventing overloaded hosts from impacting service reliabilty and providing an entry point to mitigate large SEVs
   quickly.
 - Reduced p99 latency by 50% on DIMS, and automated heap dump collection on FULLGC events
 - Reduced build failures by 30% by eliminating a critical concurrency issue in a Python capacity library
 - Removed a consistent pain point in C++ development by correcting the ephemeral build lifetime and extending the lifetime of test clusters
 - Allow automated detection of regional drain tests, reducing critical notifications by 1 per week
 - Modernize parameter storage for forecasting operator, preventing the breakage of 23 forecasting data pipelinesi
 - Document and prioritize potential impact from cluster turnup improvements to align with AI enablement initiatives
 - Led effort to reduce push failures from 70% to 5%, eliminating a major cause of oncall pain
 - Drove C++ from a production readiness perspective launching with instance health checks, capacity attribution, continuous push,
   and integration testing.
> Tyler played a critical role in multiple SEV mitgations regardless of whether he was oncall. 
> His dedication, prompt response, and generosity to offer help are deeply valued. -- Peer feedback
- **Data Infra SEV Review Core Team**
 - Plan and moderate weekly incident management review on an org-wide level
 - Contribute to fruitful and productive incident management by driving followup conversations, collecting impact metrics,
   and proposing improvements to testing and mitigation strategies across diverse services.
 - Shared learnings from other teams to drive service improvement within Data Ingestion
- **Led Config Safety Lockdown for Ingestion**
 - Audited and narrowed down aread of highest impact and completed all safe config rollout work for Scribe Ingestion services, resulting in ~156 diffs
   canaried per day.
 - Audited configs for DIMS, created a task breakdown, and completed critical tasks, allowing peers to contribute effectively
- **Release Maturity Improvements**
 - Led end-of-half release improvement fixathon, using common health check framework to reduce release validation time by ~2 hours per check

- **Technical Mentorship**
 - Mentored three junior engineers or career growth and working through technical blockers.
 - Coached four interns to successful completion of projects resulting in return offers, often through difficult pivots and
   careful delivery of timely constructive feedback.
 - Completed ramp-up as an Intern Director and shadowed summer Intern Directors through calibrations
 - Unblocked 1MW of efficiency work through load-test automation and autoscaling
> Tyler is core to the success of the DI PE Team. His curiosity about Meta systems and willingness to jump on 
> any task has lent him extensive knowledge on just about every aspect of FbETL and related systems. This makes him an excellent advisor
> on the teams' projects, as he's able to see how they fit into th data ingestion ecosystem and impact the system. Lately, I've appreciated his efforts
> to improve how the team addresses SEV followups. We didn't have a good process and Tyler built one from scratch.




## [Buddy Platform](#buddy-platform)

### Engineering Lead &mdash; February 2018 - December 2018
- Introduced REJI (Rapid Engineer Joy Index) a 0-5 quick assessment of three
  dimensions of job satisfaction during standup
- Conduct weekly 1:1s with direct reports
- Lead daily team standup
- Contribute to mobile development using React Native
- Lead design, development and deployment of Feeds, a portfolio concept to
  allow grouping and basic aggregation of energy data into defined logical
  entities to support three-phase circuit monitoring using Elasticsearch
- Design and implement graph database to implement portfolio service to
  flexibly handle arbitrary entity depth, ACL and role-based security with
  inheritance
- Design ingestion pipeline composed of four independent dropwizard
 microservices, deployed on Marathon/Mesos and communicating using Azure Event
 Hubs and Avro serialization
### Senior Software Engineer &mdash; Jan 2014 - Feb 2018
- Refactor time series database architecture into polymorphic implementations, selected based on a 3-space of external system, flow/consumption family, and pulse dimensions
- Implement weekly deliverables grooming with velocity tracking to deliver predictable progress
- Modify scrum process based on feedback from team into a kanban based process with work in progress limits
- Led weekly standup with Seattle Engineering team and report daily progress to stakeholders
- Design and implement prototype alerting system based on Kapacitor, internal webhooks, and an Incident Observer architecture.
- Design and develop a dropwizard based REST API and backing micro-services deployed using Marathon/Mesos to deliver an functioning energy monitoring prototype in three months
- Hire and develop engineering talent, driving adoption of scrum on Seattle team
- Architect and manage pluggable data processing pipeline based on the Apache Spark stack
- Build and deploy TypeScript and Libuv based MQTT front-end, enabling scalable device push architecture
- Designed and implemented CoreOS system architecture using concepts from immutable infrastructure to deliver rapid deployments and rollbacks and reduce Azure spend 30%
- Designed and implemented DataSource/DataSink pipeline for creating composable data transformation objects that can run across computing platforms
- Integrated NewRelic metrics into Stream Processors allowing custom dashboards and alerting around event stream performance
- Using beeswithmachineguns, ran load testing and profiling, identifying hot
  paths in the production web service and optimizing them
- Maintained .NET/Android/iOS/JS SDKs
- Ported JS SDK to Node.js
- Migrated MongoDB cluster to LVM/LUKS/RAID-10 configuration backed by Azure
  premium blob storage, ensured future deployments are set up properly by
  writing Chef recipes for provisioning. During testing, opened pull requests
  in upstream
gems, changes merged into Chef 12
- Managed MongoDB indexing strategy, optimizing access time for raw and  
  aggregate data
- Assist customer integrations with push notifications, guiding partner developers in using Buddy APIs to deliver pushes and monitor performance
- Redesigned telemetry architecture using an asynchronous stream architecture, allowing telemetry manipulation, filtering and recording to happen in parallel and without blocking the request thread
- Architected and implemented extensible state machine model of push notification registration and delivery transparently spanning Azure Notification Hubs and Amazon SNS and supporting GCM, WNS, MPNS, and APNS with a single REST endpoint
- Designed, implemented, and maintained microservice based continuous deployment pipeline using TeamCity, Node.js, and Chef

## [Amazon.com](#amazoncom)
### Web Development Engineer, Wireless CX Team &mdash; Sept 2011 – Dec 2014
- Redesign wireless plans and options page to use reusable JSP taglib
  components and an extensible decorator pattern for applying cart selections
  and account snapshot defaults. Use memoization and caching to reduce service
  call latency.
- Built JSON renderers into unit testable entities bound to immutable
  interfaces, allowing Javascript to adhere to a contract with Java code.
  Ensure rendering code meets 80% minimum line coverage and 75% minimum branch
  coverage standard.
- Converted all PUC pages to DataProvider architecture, allowing decoupling UI
  from dependent services by injecting static data through spring.
- Enable selling MBB (Mobile Broadband) devices though wireless detail page,
  while decoupling detail page Javascript into loosely coupled views and
  controllers, communicating using custom JQuery events.
- Implemented accessories page in PUC, allowing business users to promote
  accessories using runtime configuration, creating unit­ testable, reusable
  accessories shoveler tags. Bind shovelers to backing data stores though a
  standardized ShovelerDataSource interface, allowing external teams to
  override presentation or data binding logic.
- Managed migration from a BDB artifact for localized strings to Localization
  Metadata Service, reducing the time needed to push string revisions from 2
  weeks to 15 minutes.
- Work closely with Clickstream and Content Optimization Engine teams to debug  
  missing OPS metrics, allowing business to prioritize campaigns based on
  hourly conversion attribution data.
- Implemented Jasmine testing for client ­side media, allowing developers to
  easily write unit tests for Javascript resources
- Reduced perceived latency of UI actions by batching together AJAX requests
  and sending them invisibly while performing intermediate price computations
  on the browser, resulting in a responsive user interface that presents
  accurate and current data while preserving the customerʼs selections on the
  server.
- Drove migration from CSS to SASS, allowing more rapid style changes.
- Increased code coverage of key library packages (AlohaAppsLib and  
  AlohaPUCLib) by 20% and 15% respectively.
- Implemented PUC (Phone Upsell Cart) additional phones page, including JS for  
  adding/removing phones
- Migrated amazonwireless.com to amazon.com, creating a unified shopping
  experience for contract phones on the retail website.
- Implemented Verizon Share Everything plans, working around limitations within
  remote catalog services to create relationships between device type and
  device access fee, allowing Amazon to continue to sell Verizon transactions.
- Mitigated risk of failure by building transaction­ specific feature gates and
  testing using production data.
- Implemented configurable zip code driven tax display system to inform
  customers of the tax policies of certain states, allowing accurate tax
  information to be displayed to customers in California.

## [Health Plan Services](#health-plan-services)
### Senior Web Developer &mdash; Sept 2009 – Sept 2011
- Lead architecture, design, and development of initial implementation of a mobile quoting application for iPad and iPhone using XCode3 and Cocoa Touch built in Objective-­C and PHP using a SOAP data layer and the Strategy pattern with a single QuoteDataSource protocol used to provide a flexible path to extend and add multiple rating engines. NSInvocation callbacks allow the data source to asynchronously notify observers of changed state without tight coupling or blocking the UI. Final application consists of 5 subclasses of UIViewController which drive the application functionality and 2 data source objects, extending NSObject and implementing the QuoteDataSource protocol. Project uses the UINavigationController with a controller stack. Interface Builder NIB files define the shared data source instance via the application bundle for easy reconfiguration of the application without modifying code or recompiling.
- Foster an organizational push for test­-driven development and continuous integration using PHPUnit and CruiseControl with the goals of reducing incidence of integration defects and reducing development time for new carrier implementations.
- Propose structural changes such as dependency injection and protected factories to support mock­ driven testing practices
- Collaborate with teammates to design and implement an internal rapid web development framework (W1), constantly evaluating patterns for potential reuse and lower maintenance costs.
- Design and implement PDF views for ESSDR using the PDF Blocks plugin for PDFLib and a XML to PDF block mapping domain specific language implemented using PHP and SimpleXML.
- Together with two other senior developers, design and architect a modular and extensible enterprise enrollment system used by Cigna, Beazley and Freelancers Union (ESSDR) utilizing a set of run-­time interchangeable service ­layer modules adhering to a common interface and using the Strategy pattern and schema ­validated XML for resource loading and configuration.
- Built Observer ­based SINEWE plugins for logging and batch execution flow and scheduling.
- Build and maintain PHPUnit test cases for SINEWE components.
- Lead architecture, design, implementation, and testing of an event­-driven workflow engine (SINEWE) for tracking and restoring user state across web interfaces based on principles observed in Spring Web Flow and BPEL, implemented using SimpleXML in PHP, a Facade pattern for interaction and an Interpreter pattern for parsing workflow definitions into expression objects.
- Manage unit testing, test plan creation and defect resolution of feed generation process during SIT and UAT phases.
- Led design and development of a database configurable PHP controller class to produce a daily feed of TIFF images retrieved from an internal Stellent server for nightly delivery to Humana.
- To support feed generation class, design and implement a PHP ImageUtil class which abstracts image conversion, appending, resizing and provides error checking across multiple file formats.
- Manage unit and SIT for shared billing code to determine cross ­carrier impact pre­-deployment.
- Alter shared billing module to allow final bills to be rerun without reinstating cases across all carriers, configurable through database­ provided business rules.
- Led design and implementation of cross­-carrier database­-driven role­-based security model using existing SecurityRuntime class.
- Developed a shared module for common web portal functionality including user login, password reset, password hint, and profile settings. Rapidly configurable using static templates and XML files to access several different DB2 tables for authentication.

## [University of South Florida](#university-of-south-florida)
### Research Software Developer &mdash; Sept 2010 - April 2010
- Collaborated with researcher to develop a basic framework for building and configuring psychometric tests based on commonly changing test parameters.
- Apply a State pattern to encapsulate test trials and responses within test blocks, and to represent sets of criteria to be evaluated.
- Use the Mediator pattern to load controllers and views for diverse test phases governed by a plist XML configuration file describing the test phases without tightly coupling phase view controllers, this allowed the researcher flexibility to adjust study criterion, stimulus presentation, and program flow during testing without modifying or recompiling the application.
- Utilize the CoreGraphics and Audio APIs to deliver feedback in the form of configurable sounds and colors to study participants.
- Using Appleʼs KVC (Key-­Value Coding) pattern, designed and implemented a runtime XML configuration to access properties of stimulus objects dynamically
- Save collected data to disk as plist XML for parsing and analysis.
- Construct performance testing framework using OCUnit to ensure that response latencies were recorded within acceptable levels of accuracy.

## [Verizon Business](#verizon-business)
### Software Systems Engineer IV &mdash; Jan 2009 - Sept 2009
- Contributed to high-­level design of PHP5 class composition for abstracting revisioning and
  workflow of generic template­-driven web­ documents, utilizing database transactions and
  foreign­ key constraints to maintain consistency.
- Designed database schema and foreign­-key constraints for 7 tables supporting document
  revisioning engine classes.
- Employed document revisioning classes to create a living Business Requirement document that
  provides document workflow and traceability of user changes across revisions.
- Tuned slow queries on tables requiring MySql text columns by indexing on a composite key of
  crc32 checksum and string length and by replacing text columns with a foreign key into a
  single shared text values table.
- Designed and implemented session-­based metadata caching layer to store template specific
  data on web servers taking load off the database and providing speed improvements of 10­-15
  seconds when retrieving large datasets.
- Utilized Xajax library to allow requirements writers to modify web­-based documents
  in­-place without using synchronous operations. Extended existing document classes to
  provide partial display templates for updating page elements.
- Extended user request classes, providing generic callbacks to allow routing of user access   
  requests to appropriate decision makers and automating actions on request approval.
- Using improvements made to Request class implementation, redesigned FAAS (Firewall Access
  Authorization System) request process to automate director approval and ticket creation.
- Consult and assist developers on design and implementation of a new database class to handle
  prepared statements while maintaining backwards compatibility with existing code.
- Prepared the IPM suite for enterprise deployment by implementing input validation classes
  and query parameterization using PHP and MySQL on an existing code base of more than 600,000
  lines and supporting 13,000 active users.
