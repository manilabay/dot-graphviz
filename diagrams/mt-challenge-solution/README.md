
# MT Architecture Deliverables Artefacts

MT put a challenge Case Study for Raul Andres, this document is the artefacts delivered to MT. Raul Andres create a new project dot-graphviz-aws repo to generate architecture diagrams on fly and reuse it to work in any architecture task as a base to governance and maintain Business and Technology Architecture workflow.

MT represent a real company, but author masked it due interview confidential materials and process.
The Case Study isn't deployed for same reasons.

# Envelop project: dot-graphviz-aws
This project is another PoC by Raul Andres to create an amazing idea to generate Architecture diagrams using dot language + graphviz + aws icons + git . Lets start to create and modify Architecture diagrams in agile way! ;)

the envelop project is:
[dot-graphviz-aws](https://github.com/manilabay/dot-graphviz-aws)

created by [Raul Andres](https://github.com/manilabay)

## Solution Approach

The approach is a complete Cloud solution using AWS provider and using all the AWS components needed to support all the requirements in the MT Case Study: 4YE

Most of the components are Serverless Architecture, so it isn't required to have an own Infrastructure and maintain it.

## MT-logical-architecture  

![MT-logical-architecture](mt-logical-architecture.png?raw=true "MT-logical-architecture")

Basically and to understand very clear the diagram:

* Green arrows represent end-to-end solution User traffic
* Blue arrows represent internal processing traffic
* Red arrows represent update/release traffic

## MT-technical-architecture  

![MT-technical-architecture](mt-technical-architecture.png?raw=true "MT-technical-architecture")

Basically and to understand very clear the diagram:

* Green arrows represent end-to-end solution User traffic
* Blue arrows represent internal processing traffic
* Red arrows represent update/release traffic

All the items starting with aws_* are AWS resources

At the Application Elastic load balancers(aws_aelb) and ECS tier it could be multiplexed in to multiple albs and ecs nodes depends of the deep details and requirements for the project. I ommit to draw multiple albs and ecs nodes to do the graph basic.

The author put 2 options alternatives to the CI-CD for the solution because maybe the customer have already the CI-CD developed and Operations defined so they could choose between CI-CD pipeline with Jenkins or Bamboo as they have already or use AWS CodeBuild and CodePipeline(This part could be done also by Terraform)

The AWS Cloud Infra Automation is out of scope of this architecture artefacts and to dont mess the diagram I didnt put a Terraform arrow to every AWS resource in the picture, so it basically is to use some AWS Schema Automation tool as Terraform to automate the creation and maintain of all the AWS resources involved in the solution.

## High level risks

MT note: High level risks that you see in such a program

The CI and CD for the whole solution must be agreed with the partners solutions and third party involved.

This solution approach over use AWS, so the teams and external teams and systems involved must be mature or have the mature the agile methods to grow organically with it.

It is mandatory to have a Cloud Architect involved in the project and act as a lead for the whole solution with skills to integrate base current Architecture and convert it to this target Architecture. The Cloud Architect will work mainly with Operational(SysAdmin and Network), Developers and Business teams.

## Architecture views

MT note: Any other architecture views that you perceive as being relevant

This Architecture approach is a target Architecture, some parts of the Architecture will hybrid with current Architecture and integrate with multiple systems don´t appear in this Architecture viewpoint, because the current Architecture is unknown, it isn't defined in the Case Study.

This Architecture diagrams allow to modify on fly and track the architecture changes along the Solution Roadmap and the SDLC involved.
