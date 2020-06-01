---
title        : OWASP Juice Shop Deep Dive - MultiJuicer
track        : OWASP Juice Shop
type         : user-session      # working-session, user-session, product-session
technology   :
topics       :                    # for example ["GDPR"]
featured     :  yes                  # review with summit team "yes"
when_day     :  Mon
when_time    :  WS-3
room_layout  :                    #
room_id      :
session_slack: 
status       : draft              # draft, review-content, done
description  :
organizers   :
    - Jannik Hollenbach
    - Robert Seedorff
participants :
---

OWASP Juice Shop is an incredible tool to learn and teach about web
application security. The Juice Shop lets people attack a real(ish) web
application - which looks like a normal eCommerce Shop - and learn step
by step about some of the most impactful vulnerabilities.

When you are running a Security Training for developers based on the
Juice Shop you have one problem: How can every developer run and access
his own Juice Shop Instance to train his skills? The Juice Shop is
basically a single user application, so every user needs to have their
own instance to train.

You basically have to options:

1. You could make the users install Juice Shop on their own machines,
   which is error prone and can easily take a big valuable chunk of your
   valuable training time.
2. Or you could host all Juice Shop instances for the users.

This is where MultiJuicer comes in, an open-source Tool to centrally
host and all Juice Shop Instances for your training on a central
kubernetes cluster.

What MultiJuicer does:

* dynamically create new Juice Shop instances when needed
* runs on a single domain, comes with a LoadBalancer sending the traffic
  to the participants Juice Shop instance
* backup and auto apply challenge progress in case of Juice Shop
  container restarts
* cleanup old & unused instances automatically

In this session you will learn:

* What MultiJuicer is
* How it works
* How you can use it for security trainings either in your org, or for
  your customers
* How you track the progress of the hackers
* How you can customize it
* What features are coming in the future
* How you can get involved in the project

Audience:

* Security Educators
* Security Consultants
* Juice Shop Fanboy

