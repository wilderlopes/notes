# Wilder notes

> For context:
>
> - This is a rolling document that collects my thoughts and insights on various tech & business subjects
> - Each new "post" is stacked at the top of the document. It is dated and sometimes contains a hastag to associate it to a group of notes
> - Keep it simple

## 2023 Dec 14th

The “cloud for developers” space is getting more and more interesting. Off-loading your coding environment & computing to the cloud with the click of a button is truly what most (AI) developers want. Google collab, Streamlit, Replit are all part of most devs arsenal. And things continue to move forward – see this great tool announced by [lightning.ai](https://www.linkedin.com/posts/pytorch-lightning_lightning-ai-studios-ugcPost-7140763990384599041-XLN9?utm_source=share&utm_medium=member_desktop)  

However, we can’t forget that easy portability back from the cloud to local environments is crucial for deploying AI everywhere. A myriad of problems arise when bringing apps from well-behaved cloud environments to local (edge) production environments – you see everything from libraries that break (due to difference in OS and hardware) to apps that require manual refactoring to run outside of the cloud. 

Transitioning back-and-forth from cloud to local environments is a hard problem to solve. Overcoming that can unlock many opportunities to streamline development AND deployment anywhere.   

## 2023 Nov 12th

## Open-source vs. Source-available licenses

I have been reading all I can find about business that are built on top of code that is available for free.

Companies that choose that approach usually rely on one of the following two categories of software licenses: *open-source* (as per the definition of the [open source initiative](https://opensource.org/) or *source-available*.

These licenses differ in one key point: while both enable free access to the source code, *source-available* licenses prevent thrid parties from using the code to create a competing business offering. As explained in this great post by Vlad A. Ionescu entitled [Earthly Switches to Open-source](https://earthly.dev/blog/earthly-open-source/), *the main reason for using a more restrictive license is to prevent the competition from offering your product as a service*.

Despite the noble function of protecting the underdogs (who create and share their code with the community) against the advances of hyperscalers that want to create competing
business offers, adopting source-available licenses for dev tools creates a point of friction for onboarding new users, including enterprise users, who are not entirely sure if
they can use source-available software inside their own products. This might even culminate in losing clients. On the other hand, every company understands open-source software, and
they know they can use it inside their own offerings without risks.

The post mentioned above explores the learnings of Earthly when trying to use source-available instead open-source licenses to distribute their product. They ended up **switching back
to plain open-source** after negative feedback from contributors and clients, plus an increase in friction during the onboarding of enterprise clients who wanted to incorporate
Earthly's software inside their own offerings (without being competitors).

The **key takeaway** is: if your business can benefit from sharing the source code for free with the community, and your are developing something to empower developers, make
sure to choose a open-source license instead of a source-available.


## 2023 Nov 7th

During my career so far, and specially now as I build ogre.run, I have stumbled upon many new insights on what makes a dev tool great.

Today I ran into a post that is very much aligned with my own thinking I have been developing throughout the years: [Two types of time](https://medium.com/@graphmaven/two-types-of-time-222a1a1d3dc), by Adam Frankl (JFrog, Neo4j, & Sourcegraph).

His main takeaway is that, similarly to my own experience, *"devs hate waste"*. And waste of developer time is the worst type of waste.

This way, dev tools that focus on maximizing dev/time performance are the ones that will catch the eyes of developers. Those type of tools are essentially time machines
that keep generating extra time to devs, who can then use it the best way they see fit -- but most probably, they will reinvest this "magically" gained time into
their own projects/companies, generating more value for the entire chain.

Focus on creating time for devs -- they will love it.

