---
layout: post
title: Lead time - A key metric in DevOps
date: 2020-06-10T15:08:07.918Z
image: /images/devops-3155973_1280.jpg
categories: "DevOps "
tags: "DevOps "
---
\
*Lead time is a critical metric to enable a company to improve its speed of deployment. We take a deep dive into how lead time differs across organizations, how it can be improved, and where it fits into the greater context of improving business outcomes.*

DevOps aims to improve business outcomes within an organization through greater cohesion amongst team members and increased efficiency and effectiveness. Measuring DevOps metrics such as lead time enables a company to streamline and optimize deployment pipelines and reduce lead times to improve business outcomes.

## What is lead time?

In simple terms, the lead time is the time it takes to implement, test, and deliver code. To measure lead time, teams need to have a clear definition of when work begins and ends such as the measurable time between when a commit has been made, and the resulting code gets into production. The aim is to increase the speed of deployment through automation such as an optimization of the integration of the testing process to shorten overall time to deployment. Using [multiple development environments](https://humanitec.com/blog/managing-environments-in-a-kubernetes-cluster) ensures that software is rigorously tested prior across a range of shared, test and feature environments.

A [development environment](https://humanitec.com/blog/kubernetes-environments-basics) is a space where devs can deploy code and test any newly implemented features. Bugs can be dealt with early on. Once the code is largely stable, Quality Assurance tests can be performed to detect any new bugs and run performance tests. This loops back with the development environment to fix the bugs identified and any areas for improvement. Once the code has been thoroughly tested, it can be pushed to production where it is made available to end-users.

Lead time is a clear metric with which to measure if/when team deployments are increasing in a way that can be understood by the team and any external customers.

The lead time clock starts when the request is made and ends at delivery.

## Why is lead time an Important DevOps key metric?

Lead time is a way to gain valuable insights into the efficiency of the development process. Within a team, lead time metrics can measure the deployment frequency of team members, and their level of skill. Within a company's objectives, it represents how responsive the company is to customer or user needs. A long lead time may suggest a team experiencing bottlenecks, or it could be in mean a company prioritizes more complex project requiring more time - both are important factors to consider

## What is that state of lead times?

The [2019 Accelerate State of DevOps Report](https://services.google.com/fh/files/misc/state-of-devops-2019.pdf) provides some interesting insights into lead times.

Survey respondents were asked: "For the primary application or service you work on, what is your lead time for changes (i.e., how long does it take to go from code committed to code successfully running in production)?"

Lead time was categorized as: 

* Less than one day (Elite)
* Between one day and one week (High)
* Between one week and one month (Medium)
* Between one month and size months (Low)

The elite group (20% of survey respondents) reported that it routinely deploys on-demand and performs multiple deployments per day. By comparison, low performers reported deploying between once per month (12 per year) and once per six months (two per year).

Elite performers deploy code 208 times more frequently than low performers. The research also notes that companies such as CapitalOne report deploying up to 50 times per day for a product, and companies such as Amazon, Google, and Netflix that deploy thousands of times per day (aggregated over the hundreds of services that comprise their production environments).



"With lead times of 24 hours for elite performers (a conservative estimate at the high end of "less than one day") and 2,555 hours for low performers (the mean of 730 hours per month and 4,380 hours over six months), the elite group has 106 times faster change lead times than low performers."

## How to reduce lead time?

There are a couple of essential ways to reduce lead time:

### Automate the Deployment Pipeline

Automating the deployment pipelines of building and testing facilitates continuous delivery and substantially shortens lead time. Tasks that were traditionally achieved manually, including security and compliance benefit from the efficiency of automation.

Automation involves two central processes: [Continuous Integration (CI) and Continuous Delivery (CD)](https://humanitec.com/blog/continuous-integration-vs-continuous-delivery-vs-continuous-deployment). CI means that devs commit code (integrate code) into a shared repository frequently. Each commit can trigger an automated build of an artifact. This step also contains automated integration tests.

CD means that you should be able to deploy at any time. In the continuous delivery process, you deploy to all dev environments incl. staging automatically but not to production. Automated deployment to production would be Continuous Deployment.

### Release little and often:

A long lead time means the risk that your efforts at leading-edge innovation may not be all that new or exciting by the time they reach the customer, and faster-moving competitors may have usurped you. Many industries move fast, and you may struggle to respond to any changing business needs.

With Continuous Delivery, you can release each feature as it is ready rather than waiting for an 'all-in' big release, substantially reducing lead time. A chain of smaller releases keeps customers happy and faster; smaller releases make it easy for developers to modify their work in response to customer feedback.

## It's not a precise science

Lead time as a measurement of efficiency is something which can vary widely across organizations depending on factors such as team size, the skill, and the workload of each developer. It’s not about using it simply to measure the work of individual team members - it would be unreasonable for a team of junior developers to achieve the elite metrics of very experienced developers. Further, many devs wear several hats at work and may have different priorities of wear to concentrate their attention. But it can be used to look at the workload of an overall team and discover bottlenecks such as lengthy approval processes, understaffing, or poor resource allocation and provide the catalyst for efforts to reduce delays and lower meantime.

Further, there's no value in increasing the speed of output if the outcome is a sub-optimal product that requests extensive fixes. DevOps aims to optimize the business outcomes of an organization, and quality control is critical to company reputation and commercial success.

## Conclusion

Reducing lead time is critical but equally important are the metrics of deployment frequency, mean time to restore (MTTR), and change failure percentage. One of the benefits of DevOps is that it's a way of thinking rather than prescriptive steps or practices. This means it's malleable and adaptable to specific organizational culture, processes, challenges and goals. DevOps enables an organization to forward their goals and increase their quality of product and customer service.