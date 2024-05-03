---
title: infrastructure as a code
date: 02 May 2024
description: irrelevant interview question? here you go...
keywords: infrastructure, iac, code
draft: false
---

<!-- happy new year! 🎉🎈 <br>
[wanna say hello?](https://x.com/1cbyc) -->

i think it is now time i talk about infrastructure as code (some interviewers ask these days; it isn't necessarily an irrelevant question in case you come across iac).

anyways, infrastructure as code is just an idea in the cloud stuff and infosec. it is just about defining and managing IT infrastructure through code rather than relying on manual processes. so, iac is literally a significant shift in how we handle and operate infrastructure resources, to allow us enjoy automation and scalability.

**anyways, some of the reasons i would suggest iac includes:**

**consistency:** iac allows your infrastructure to remain consistent across various environments (like dev, staging, prod), so you don't even have to deal with manual errors and ensuring that the infrastructure is provisioned consistently each time.

**version control:** by treating your infrastructure as code, you can track changes to it infrastructure just like you would with application code. this makes it easier to identify issues and revert to a previous state if necessary.

**collab:** iac allows team members to engage each other faster, even if it is to define and manage the infrastructure. who doesn't like better communication and visibility within the state of an infra?? 

**automation:** iac enables you to automate the provisioning, configuration, and management of infrastructure resources, reducing the time and effort required for provisioning and allowing you to scale your infrastructure quickly in response to demand.

while getting excited, there are tools we use for iac, though the **most common tools** are **terraform, aws cloud formation, azure resource manager templates and even google cloud deployment manager.**

**

there is no way i'd talk about anything in tech without telling you about their **best practices**. in fact, i enjoy writing best practices documentations.

my top iac best practices involves **using version control** to store your iac files and even to track changes. it also involves actively **breaking down your infrastructure code into smaller and reusable modules** that can be shared and also combined to create more complex infrastructure configurations (some of us like simple things, explanation is hard for me).

i am also a big fan of **validating and testing back-to-back** even if it is unit tests and static analysis; atleast to ensure the correctness and security of your infrastructure code before deployment. it is only right to **continuously monitor and update your iac code** (nothing is permanent now, even God had to make new versions of humans - the ones they call gen z).

> [!NOTE]
> you can also ask me specific questions about building your own infra and anything on infrastructure as code.
