---
layout: post
title: DevOps Enterprise Summit shows the reality of DevOps across industries
date: 2020-10-23T15:00:05.262Z
image: /images/5f92c7bf6ca09902c553481a_devops-enterprise-summit.png
categories: "developer tools "
tags: DevOps
publication_url: https://humanitec.com/blog/devops-enterprise-summit-las-vegas-october-2020
---
The second DevOps virtual summit was recently held this year (a necessary departure from its usual home in Las Vegas). It’s a conference for the technology leaders of large, complex organizations implementing DevOps principles and practices. Founded by [Gene Kim](http://www.realgenekim.me/), the event’s goal is to give leaders the tools and practices they need to develop and deploy software faster. The programming emphasizes both evolving technical and architectural practices and the methods needed to lead widespread change efforts in large organizations.

While attending a conference virtually can’t compete with the pizzazz of the Las Vegas Strip, the conference is a great one for open and honest sharing around [DevOps](https://humanitec.com/devops) successes, failures and enterprise of digital transformation.

We recently attended and wanted to share some of the takeaways from the various talks with you.

## Team Topologies in Action: Early Results from Industry

*[Team Topologies](https://teamtopologies.com/),* authored by Manuel Pais and Matthew Skelton hardly needs an introduction. The book was published in 2019 and organizations around the world have started to adopt *Team Topologies* principles and practices like Stream-aligned teams, modern platforms, well-defined team interactions, and team cognitive load as a key driver for fast software delivery and operations. We’ve previously [detailed some of the specifics](https://humanitec.com/blog/devops-enterprise-summit-london-2020) of  the concepts that underlie *Team Topologie*s after the previous DevOps Enterprise Summit earlier this year.

Mathew asserts that key problems team topologies aims to solve include:

* Why is our transformation not achieving fast flow
* What’s our purpose admission as a team within the wider organization
* Why are our teams not able to respond quickly to business needs? 
* How can we safely remove low level complexity from customer facing teams

Manuel and Matthew shared the journey of the footwear company Footasylum:

### Case study: Footasylum 

Footasylum gives fashion-focused youth a multi-branded retail experience mixing global sportswear household names with emerging brands and its own stable of in-house labels. Founded in 2005, Footasylum now has 70 stores across the UK and a thriving ecommerce platform, with revenue of £260m per annum and over 2500 employees. Footasylum used Team Topologies patterns to revolutionize their ecommerce platform.

### The problems with team dynamics at Footasylum

Historically, a piece of work would start with a Senior Product Manager, who would in turn give this to a team of Product Managers, each of which would then assign the task to a developer. The teams boundaries were drawn up by their location, instead of the product they worked on. The IT department in the U.K. was made up of 27 people across development, product management, support, infrastructure and data, while there were over 40 people in teams in Romania and India. The work was assigned to individual developers, with a handover of work from a Product Manager team to the development team. This formed not only a constraint, but also a complex communication path for context to be lost in.

Individual developers were responsible for features and bug fixes, as well as being directly contacted by people in other departments. This led to the priority of work changing to meet the short term need of frustrated colleagues, instead of focusing on a wider business outcome and creating transparency and a closer working relationship.

Manuel recalls “There was a high fragmentation of work and projects with the priorities of software devs changing on a short term basis depending on who was the most frustrated and it prevented a lack of focus on wider business outcomes. Further, the cognitive load off individual devs was high because he  had to work with many different languages.”

Constant context switching meant that features were half implemented, which led to a brittle system where shortcuts were taken and technical debt accrued. “The trade-offs for not paying down this debt meant that creating safe systems would be sacrificed in order to deliver to deadlines.”

### The way forward

Long story short, a number of strategies were developed over time, some of the key actions include:

The first step of reorganising the teams was to identify boundaries between each part of the business from a domain point of view, and create small product teams to align to a business unit, with the ability to work independently of other teams.

The service team later renamed themselves the Platform team’s an worked to start breaking up the complicated legacy backend systems that shared a database - into components that could be individually deployable. Increasing safety was their primary goal at this point, building quality in at an early stage by adopting a lean, loosely-coupled, test-driven approach. 

The team also focused on Simon Wardley’s [Pioneer/Settler/Town Planner framework ](https://aktiasolutions.com/introduction-to-wardley-maps/)recognising that pioneer services would be their TVP, with the Platform team giving the Stream Aligned team static data via a simple API endpoint, or access to a sandbox environment on Azure. They could build the minimal service themselves, and as they validated assumptions and needed to grow the service, the interaction would change from X as a service to collaboration.

It’s been 13 months since *Team Topologies* was published. Forever an example of  dynamic documentation Matthew shared learnings since the book’s launch:

“The streamlined team is the starting point. It provides fast flow and feedback from running systems. Further, we need to design specifically for team cognitive load.  A platform is a curated experience for engineers to accelerate and simplify software delivery. Don’t obsess about the technology in the platform, think about the experience of those using the platform first.”

### Free team topology resources 

* [GitHub.com/teamtopoloiges](https://github.com/teamtopologies)
* [Teamtopologies.com/remote-first](https://teamtopologies.com/key-concepts-content/remote-first-team-interactions-with-team-topologies) (the authors are currently working on a workbook)
* [Modeling Shapes for Team Types and Team Interactions (PDF](https://teamtopologies.com/shop/modeling-shapes-for-team-types-and-team-interactions-pdf?rq=modeling))

[![Take the DevOps Maturity Test](https://no-cache.hubspot.com/cta/default/5890440/68850f86-c19a-47a1-b6b7-0eb3e291015c.png)](https://cta-redirect.hubspot.com/cta/redirect/5890440/68850f86-c19a-47a1-b6b7-0eb3e291015c)

### My Ops Team Can't Keep Up with My Dev Team

Dave Mangot, principal at [Mangoteque](https://www.mangoteque.com/) gave an interesting talk about the frustration of the inability of Ops to keep up with Dev in today's fast paced cloud model. There are a number of general principles that are often the solution for many of the problems. 

He shared the challenges of working with Cassandra, noting “we were running at 70% utilization. Pain points included:

* Many outages
* Recovery could take days from a failed node
* Complicated and fragile configuration
* Expert level knowledge mandatory for recovery

He notes: 

“Our response was to upgrade. However upgrading made things worse. We were getting massive time outs. So we were left to figure out where the problem was introduced. We thought it would be easy to test between the two versions of Cassandra via GitHub and discovered that there were 5827 commits between the version that we were on, and the version we wanted to go to.”

Fortunately, the team were able to use Git bisect to find out the actual problem.Git  bisect enabled them to propose random commits e.g. 3000, 1000 to determine if the problem was before or after the respective commit number.

“However Cassandra rings could take days to hydrate if there was a problem. As an SRE team we created the ability to stand up a Cassandra ring in 20 mins. And isolate the exact commit causing the problem in 2.5 days. We wrote a patch, and it fixed the problem.”

Dave asks, “But how many organizations can really do something like this? What would you have done if we hadn’t developed the ability to stand up a full Cassandra ring in 20 mins?: “

* Never would have tried
* Maybe hire consultations
* Done something else

He asserts, “Coming together to solve the problem is the essence of DevOps. Our ring recovery has gone from days to minutes benefiting many in the organization. We were also moving across AWS and reduced our costs.” The team was eventually able to create a stand up solution that replaced Cassandra entirely, saving 70% in costs.

### How does MY ops team do that? 

According to Dave the two critical component of an SRE role are:

* Keep the site up
* Keep the developers moving as fast as possible

He spoke about empathy and the notion of prosocial concern, the feeling we get when we recognize someone else is in a situation that we can help, suggesting keeping the site up is an example of prosocial concern.

He also suggests that the ticketing system needs to be burnt as a pain point of toil. Toil is about identifying and containing work that takes up our time, blocks people from fulfilling their engineering potential, and doesn't move a company forward. He notes that:

“Remediation work is just work. It's the opposite of toil, we elevate this kind of work. However failure is just part of regular work. Work is not linear and you can’t ‘action item’ your way out of a problem.”

He further asserts that organisational debt often manifests erroneously as tech debt. 

“Tech debt should be a conscious choice . It can be monitored through 

OKRs (Objectives and key results), visions, values and leadership who communicate what's most important to the organization in order. Have operations and engineering under the same leader to avoid individual silos and the risk of tech debt.” 

## Psychological Safety and DevOps

You’ve probably seen the subject of psychological safety pop up at developer conferences over the last few years. [PeopleNotTech](https://www.psychologicalsafety.works/) designed a solution to measure and increase Psychological Safety by working with hundreds of teams around the world -in particular in financial services. Duena Blomstrom, Author, Co-Founder and CEO of PeopleNotTech and Ffion Jones, Partner gave a presentation about what is psychological safety, what are the benefits and what works and doesn’t. 

### What is psychological safety?

![](https://assets.website-files.com/5c73bbfe3312822f153dd310/5f92c4c65b82d831483d8456_eT-FRZbzLG7foW7YYo7kY3RTWLBs-KYFgIRoptDqyVZasPAy-c9u5u4x1HBQ0yzfrC3qRSh1E9aHVjqaqamO-BTOlhErAeATe5Hq_hDvRQ0Zx4Ut_m3VTEpwwZEWq-5noJHCc0Y4.jpeg)

Source: Duena Blomstrom/Ffion Jones



There's a number of definitions of psychological safely but the main one is:

“Being able to show and employ oneself without fear of negative consequences of self-image, status or career.” (Kahn 1990)

Google’s infamous [Project Aristotle](https://institutesuccess.com/2020/01/what-is-project-aristotle/) ran over four years with over 50k people surveyed, 180 teams, and 100 + variables. Duena notes “ALL data showed the most important lever of high performance to be Psychological safety. Similarly, Accelerates State of DevOps annual research demonstrates that you can’t be a top agile performer or digital elite without psychological safety.”

### Remember Nokia? 

They flew high in the 90s as a cell phone manufacturer but lost most of their market value in 2012. A Harvard study revealed the executives were talking about the emerging threat (google and apple), and manager and execs weren’t telling bosses that tech couldn't compete in an emerging market. Thus they missed the opportunity to compete and became irrelevant.

Ffion shares how the company tries to fix the problem: 

“The HR dept vowed they would make people speak up. So they sent one HR rep to every stand up and asked devs to choose a task or ticket and tell everyone how they felt. Such an approach creates more fear and more impression management than psychological safety."

### The trouble with Impression Management

Impression management is the effort to control or influence other people's perceptions. This could be their perception of a certain person (including you), a material possession or an event and the desire to favourably control other people’s impressions.

In one research study. C-suites were asked to keep a journal the day before an important meeting to track their thoughts. It was found most were thinking about their appearance at the meeting, workplace politics, and the opportunity to network. Under 10% thought about the content of the meeting. 



### How to foster great psychological safety at work: 

![](https://assets.website-files.com/5c73bbfe3312822f153dd310/5f92c4c603a8132b5ae188c0_DOQk34U0CxG4iWzrVQ10qM-2FqPUltC-_EGKIUH885QC67mvVhmMlHI1YFv4ZtWl5fN100xXDfbooI0j3O5TyxEEKD2UiOquRptBC4I85JSoJqx8EUCOEVM-4VXiGV62vYtHJj-G.jpeg)

Source: Duena Blomstrom/Ffion Jones



Duena and Ffon offered a number of key takeaways:

* Emotional intelligence training for tech leaders
* Make psych safety in teams one of your OKRs. Needs to be as tangible as a company’s financial goals 
* Role model at a high level - e.g. psychological vulnerability. Saying I don’t know, team leaders talking openly about importance of a speak up culture 
* Protect the psychological safety bubble of your team 
* Make psychological safety the cornerstone of team conversations

All in all, it was a fantastic event, with plentiful presentations, a highly engaged audience (never seen so much slack chatter during a conference) and plenty to demonstrate the DevOps is alive and kicking.