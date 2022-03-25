# monitoring_and_cd
## Context

A monolithic application will be split progressively into multiple services.
Each service can be managed and developed by independent development teams. The goal of this transition is to give flexibility on the deployment process and delivery calendar, to improve the feature scaling and growing, to secure services interaction, availability, and scalability to provide a qualitative service to customers.

## Challeges
Delivering multi-services that can interact between them require stimulating some concept to be safe and confident in the features delivery process:

*continuous service deployment
* integration testing
* cost management
* service and infrastructure monitoring
* troubleshooting
* incident management
* service level objectivation
* autonomous and responsibilization of features teams
* service performance, rate-limiting, and quotas management

In this study, I only cover concepts related to service continuous delivery and service monitoring but other concepts can be introduced depending on the service criticality and teams maturity.
Those other processes can be introduced either at the beginning of the continuous delivery implementation or just after in a continuous improvement process


## Roadmap
Delivering a service require to develop the feature.
But it's not enough. A feature require to be deployed on a technical infrastructure and to interact with some techincal component or tiers services that are managed internal or externally.

The first challenge before automating the delivery is to secure the service integration on the infrastructure target. Continuous deployment testing will help to identify regressions and compatibility break between development and infrastructure.

The second challenge is monitoring all component that contribute to deliver the service. This include the infrastructure part but also the application part with technical metering, event, logs but also business metrics to anticipate feature usage growth or incident detection

The third step is to define and implement the Service Level Object to evaluate the quality of service expected. this will help the infrastructure and development teams to challenge the delivery quality and make the teams responsible for the positive or negative impacts on the quality of service perceived by customers. The service level objectification makes it possible to balance efforts between the development of new functionality and the reliability of the delivered service.

Now that the deployment is tested, the integration with tiers services is validated and the quality of service is measured, we can safely embrace the continuous delivery process.

But those 4 steps only cover the continuous delivery. This process needs to be enriched with some other aspects like performance testing, auto-scaling, and financial management of service run to cover the product cost optimization and the activity growth.


## Technical Architecture

