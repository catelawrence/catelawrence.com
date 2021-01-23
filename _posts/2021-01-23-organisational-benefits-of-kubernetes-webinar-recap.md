---
layout: post
title: Organisational Benefits of Kubernetes [Webinar Recap]
date: 2021-01-23T15:54:13.739Z
image: /images/5faadce1e4c4c94dff07f2e1_organisational-benefits-of-kubernetes_blog-header.png
categories: "developer tools "
tags: "Kubernetes "
publication_url: https://humanitec.com/blog/organisational-benefits-of-kubernetes
---
*In this article, we detail the key topics that featured in a recent roundtable discussion into the role of Kubernetes and DevOps in enterprise: understanding key principles, organisational buy-in, level of difficulty and where Kubernetes sits in terms of future innovation.*

Humanitec recently joined a virtual roundtable taking a deep dive into Kubernetes and where it fits within the DevOps culture. The discussion was hosted and facilitated by Raj Bains and[ ](https://www.linkedin.com/in/bainsxiii/)Mike Dwyer from [DevOps Berlin](https://www.devopsberlin.de/) and Magic Sandbox. The panelists were:

* [Mislav Stipetic](https://www.linkedin.com/in/mislavstipetic/), Founder and CTO, [Magic Sandbox](https://www.msb.com/)
* [Nigel Poulton](https://nigelpoulton.com/), trainer and author, [Magic Sandbox](https://www.msb.com/)
* [Chris Urwin](https://www.linkedin.com/in/chrisurwin/), VP FIeld Engineering, [Rancher Labs](https://rancher.com/)
* [Chris Stephenson](https://humanitec.com/author/chris-stephenson), VP of Product and Engineering at [Humanitec](http://humanitec.com/)

This article provides details of just some main points of the conversation. It's definitely worth checking out the video below to enjoy the whole discussion in detail.

‍

## Kubernetes offers new potential to cloud computing

Mislav describes [Kubernetes](https://humanitec.com/kubernetes) as essentially a new operating system of the cloud that “allows you to do away with the current abstractions. With Kubernetes, you can think about workloads and resources and pools of memory and CPUs. You can do away with the notion of something listening on a socket on a machine and organize your software differently in a cloud-native way."

For Nigel, Kubernetes is “the future of infrastructure as code”, akin to an operating system for the cloud where "your application can just run on Windows or Linux because they abstract all of the hard stuff underneath. 

Kubernetes does the same thing, potentially, for all the different clouds out there, whether on-prem or hybrid, and let somebody else care about that complexity. Customers are happy because it does all of the auto-scaling; it does all of the self-healing, zero downtime, and rolling updates.

Nigel is a fan of how applications are defined in Kubernetes and likes how the documentation process inherent in Kubernetes through the use of yaml:

“It uses this particular version of a container image. It operates on this particular network on this particular port. It uses this particular service account' - all of this must be documented for the application to run on Kubernetes as a platform. This leads to loads of benefits. Operations automatically get documentation in the yaml format of every application deployed. So it almost forces you to operate in more of a DevOps way. So as I'm a big fan of that aspect of it culturally."

## DevOps facilitates self-serve practices

Chris Stephenson champions how [DevOps](https://humanitec.com/devops) gives developers the ability to self-serve, and to do things independently: "The complexity of dealing with Kubernetes directly, especially when it's newly introduced can be quite high. But that kind of complexity doesn't have to be an impediment. If you structure things well, this can be very self-serving.

He notes that ideally, you want your developers and operations people to be able to perform tasks without impediment:

"As an application developer, I should be able to deploy my code. If I make an update, I should be able to get that code up and running. In Kubernetes, that's relatively straightforward. I can make sure that's running as it'll roll over easily, so I don't cause downtime. Then, maybe as an operations person, I want to be able to understand what the configuration is for my application."

## Get started with Kubernetes and DevOps in your organisation

The issue is often raised of who is responsible for introducing new technology to an organisation and how to get started. Nigel suggests testing a greenfield application that is not critical to the business using a team strategic thinkers who can take their results to the wider organisation:

 “Document how to do it and then start picking some other easy applications within the organization, and drafting in other people from wider teams getting them on board to it."

Chris Stephenson agrees to the notion of starting small and building out:

"One of the exciting things about Kubernetes is that the barrier to entry is relatively low. You don't have to dedicate a whole load of servers that you have to provision and manage yourself; you can spin things up in the cloud very straightforwardly and get started within 20 minutes.

He suggests starting with a small application for experimentation where more complexity can be added as you progress: “Add more complexity as you go on, add external data sources, add more complicated routing. Just take it step by step."

Importantly the team should be limited to engineers but should include people from operations, testing, and product managers working together to ensure that the benefits are understood and troubleshooting can be shared.

## Kubernetes is traditionally complex but help is at hand

Chris Stephenson attributes Kubernetes complexity to what it can do:

"It has 6000 contributors. The edges have a whole load of crazy things that can be done, especially in the alpha and beta functionalities. But in practice, most people will probably work as some variation of the 80/20 rule, 80% of people will be using 20% of the features."

He stresses the issue of the additional cognitive load that you introduce in your engineering team: "So if you had enterprise Java developers and you suddenly tell them to go learn Kubernetes, you might get some pushback on that. Especially kind of if you do this at scale across thousands of engineers across an organization."

Chris Urwin asserts that earlier versions of Kubernetes were much more complicated, but that there are organisations like Rancher and Humanitec that can help with the heavy lifting: “We're almost getting to that point where you wouldn't really build Kubernetes DIY yourself anymore, You just go and pick it off the shelf, whether you're on-prem or in the cloud."

Mislav believes that Kubernetes is basically becoming a set of APIs: "You don't care what's in the background, you can use something like Virtual Cubelet, and put it on AWS fargate. And you don't literally think about servers anymore. So Kubernetes just becomes this kind of flexible API for things to plug into, from different storage providers to different platforms on top."

However we are also witnessing the growth of solutions like those provided by Humanitec which are built on top of Kubernetes, and provide not only an API but also an intuitive UI. Adopting new tech needs tools and platforms which are accessible and appealing to multi-discipline teams to secure their use.

## Financial investment vs. The Kodak moment

Nigel believes that the death of former Fortune 500 companies (like Kodak) can be attributed in part to their hesitation to use and leverage new technology noting “if you don't move your product, you're going to disappear as a business."

He provides the example of VMware, asserting that if you use it over better options means "you're not going to exist as an organization in the future, because you're not going to be efficient enough." He suggests that if you avoid Kubernetes and DevOps, "The cost to your business might be that you might not be in business anymore. Or the cost to you, as an individual as a developer might be that you can only have the substandard  jobs because you haven't skilled yourself up to be able to get the good jobs going forward."

Chris Stephenson suggests that investment in Kubernetes and DevOps is a long game investment. "Commodification drives down costs and leads to standardization. It means that suddenly you can hire people that know how to do stuff with what you have. It means that when you buy something off the shelf, you need to do less work to plug it in. What you're playing for is the long game."

‍

![](https://assets.website-files.com/5c73bbfe3312822f153dd310/5fbe2acfe39d7a16fba8a260_Kubernetes%20-%20Misconceptions%20vs%20Reality.jpg)



## Why should you adopt Kubernetes?

Chris Stephenson calls Kubernetes "the new standard, it is how people are building applications today. This technology has been tried and tested with the biggest companies in the world. and it's not going to go away. If you're not on board, you're going to be missing out, you're going to have more expensive costs, it's going to be more difficult to hire people for your legacy systems. It's going to be harder to build modern applications. And it's going to leave you behind basically."

## Critical considerations when thinking about getting started with Kubernetes

* Kubernetes and DevOps have become ubiquitous at streamlining processes and building teams and their journeys points towards a strong future.
* However, Kubernetes is not a silver bullet - make sure you have a solid use case to gain C-suite support.
* Get a cross-departmental team to begin with non-essential tasks to learn by doing.
* Kubernetes is accused of being very difficult but vendors like [Humanitec](https://humanitec.com/) provide an abstraction layer to reduce complexity. At Humanitec we allow you to keep using your existing tech stack as our open API and extension points allow you to incorporate the tech and tools you're already working with.
* Eschew the technology and you risk your skills, your team, and your product becoming obsolete. 

‍