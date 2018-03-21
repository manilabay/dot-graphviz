
# Data Pipeline Architecture Reference

Deliverables created by for Raul Andres, this document is the artifacts delivered to TF to help himself in an Interview process. Cross the fingers and wish luck to him ;)

It was 1 day of work, so please assume some errors by the author or improvements to-do.
Also please feel free to send feedback via PR.

TF represent a real company, but author masked it due interview confidential materials and process.
The Case Study isn't shared for same reasons.

created by [Raul Andres](https://github.com/manilabay)

## Solution Approach

The approach is to design a E2E Data Pipeline from Data-driven, Strategy Design, Scalability, Analytics, Monitoring and Reliability viewpoints.

It doesn't include Infra Architecture and Data Security viewpoint. TO-DO

## TF-logical-architecture  

![TF-logical-architecture](TF-logical-data-architecture.png?raw=true "TF-logical-data-architecture")

The above image represent an abstract high view and logical architecture for a Data Pipeline

Basically and to understand easier the diagram:

* Green arrows represent end-to-end solution User traffic
* Blue arrows represent internal processing traffic
* Red arrows represent update/release traffic

## TF-technical-architecture  

The above image represent a deep detailed technical architecture reference for a Data Pipeline

![TF-technical-architecture](TF-technical-data-architecture.png?raw=true "TF-technical-data-architecture")

Basically and to understand easier the diagram:

* Green arrows represent events/facts/storage traffic
* Blue arrows represent internal design strategy traffic and update/release traffic
* Red arrows represent monitoring traffic
* Orange arrows represent end user visualization traffic

## Envelop project: dot-graphviz-aws
These deliverables were created using another solution and git repo created by Raul Andres to create an amazing idea to generate Architecture diagrams using dot language + graphviz + git. Lets start to create and modify Architecture diagrams in agile way.

the envelop project and repo is:
[dot-graphviz-aws](https://github.com/manilabay/dot-graphviz-aws)
