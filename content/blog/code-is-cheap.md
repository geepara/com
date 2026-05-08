+++
title = "Code Is Cheap"
date = "2026-05-05"
description = "AI has changed the cost of trying software changes. When generated code is cheap, software work can move from requests to attempted solutions."
tags = ["software", "ai", "implementation"]
+++

When code is expensive, the goal is to avoid wrong attempts. When code is cheap, the goal is to make attempts easy to generate, easy to review, and easy to discard.

This is the first article in a two-part series.

## The Cost Of Trying Has Changed

For most of software history, code was expensive.

Every software change consumed scarce engineering attention. If someone found a bug, wanted a small workflow change, or noticed something off in the product, fixing it meant taking an engineer away from something else.

That shaped how organizations handled software requests.

In the pre-AI world, if someone outside engineering noticed a bug, the workflow usually looked like this:

```plain text
notice issue -> report in Slack -> create ticket -> backlog -> prioritization -> engineer fixes later
```

If fulfilling a request requires an engineer to stop what they are doing, understand the issue, reproduce it, make the change, test it, and ship it, then the organization needs a way to decide whether that request is worth the cost. Tickets, backlogs, and prioritization exist because engineering time is scarce. When code is expensive, even small fixes have opportunity cost.

## The New Workflow

A newer workflow is starting to look more like this:

```plain text
notice issue -> report in Slack -> engineer tags devin -> generated fix -> engineer review -> merge
```

Someone reports a bug or product issue in Slack. An engineer sees it and tags a coding agent to try a fix. The agent generates a proposed change. The engineer reviews it, asks for changes if needed, and merges it if it is good.

The important part is not that the generated fix is always right. The important part is that generating the fix is cheap.

If the solution is wrong, that is okay. The engineer can reject it, redirect it, ask for another attempt, or use part of it. The organization did not spend the same amount of scarce engineering capacity it would have spent on a fully manual fix. The cost of trying went down. That is what "code is cheap" means.

## From Reporting Problems To Initiating Fixes

Today, an engineer might be the person who tags the coding agent. But the direction of the technology points somewhere else. Over time, the person who originally noticed the issue will be able to tag the agent directly.

The workflow will become:

```plain text
non-technical teammate notices issue
  -> reports it in Slack
  -> tags coding agent
  -> agent opens proposed fix
  -> engineer reviews, approves, and merges
```

Non-engineers will not need to become engineers, but they will be able to create the first draft of a solution. Engineering still reviews and approves. The difference is that the person closest to the problem can now help start the path toward the fix.

Previously, software work entered the system as a request. Now it can enter the system as an attempted solution.

## Why Wrong Attempts Are Fine

The strangest part of cheap code is that wrong attempts become less scary.

In the old model, a wrong implementation was expensive. An engineer spending days on the wrong thing was costly. It made sense to slow down, scope more, and avoid wasted work.

In the new model, the first generated attempt may be wrong, but the cost of generating it is low. A wrong attempt can still be useful because it teaches the reviewer what the agent misunderstood, can clarify the request, and expose missing context. It can become a partial starting point.

When code is expensive, the goal is to avoid wrong attempts. When code is cheap, the goal is to make attempts easy to generate, easy to review, and easy to discard.

## The Bigger Question

This shift is easy to see inside a software company. A Slack message can turn into a generated patch. A non-technical teammate can initiate a fix that an engineer reviews. But the implication is bigger than internal engineering workflows.

If code is cheap, then any industry built around expensive software change has to rethink its workflow.

System integrators are one of those industries.

Their work has historically assumed that changing software is expensive. That assumption shaped how they scope, document, align, and deliver implementations for customers.

So the next question is: what happens to system integrators when code becomes cheap?

Next: [What Cheap Code Implies For System Integrators](/what-cheap-code-implies-for-system-integrators/)
