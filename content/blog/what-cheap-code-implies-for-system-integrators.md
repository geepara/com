+++
title = "What Cheap Code Implies For System Integrators"
date = "2026-05-05"
description = "If code is cheap, system integrators can move delivery earlier and use working software as the alignment artifact."
tags = ["software", "ai", "implementation", "system-integrators"]
+++

This is the second article in a two-part series:

1. [Code Is Cheap](/code-is-cheap/)
2. **What Cheap Code Implies For System Integrators**

## Implementations Were Built Around Expensive Delivery

If code is cheap, system integrators have to rethink how implementations work.

The old implementation model was built for a world where delivery was expensive. Writing code, configuring customer-specific workflows, integrating systems, and revising an instance required scarce technical capacity.

That made the traditional workflow rational:

```plain text
scoping -> scoping -> scoping -> docs -> alignment -> delivery -> scoping -> delivery -> done
```

This workflow can look slow from the outside, but it made sense under the old cost structure.

If building is expensive, you want to be very sure before you build. If changing is expensive, you want to avoid rework. If the first version takes a long time to deliver, you want to gather as much alignment as possible before the customer sees it.

That is why implementations became so document-heavy.

Documents were cheaper than rework.

## Documents Became Proxies For Software

In the old model, documents did a job that software could not do cheaply.

They gave customers something to react to before the system existed. They helped stakeholders align on requirements, workflows, fields, permissions, integrations, and edge cases. They gave system integrators a way to reduce uncertainty before expensive delivery work began.

In that world, the implementation process naturally emphasized:

- More meetings before building.
- More requirements before configuration.
- More documentation before delivery.
- More signoff before users could touch the system.
- More change control after delivery.

The customer was often asked to imagine the future system from written descriptions, diagrams, and review meetings.

That was not ideal, but it was practical. When code is expensive, a document is a cheaper alignment artifact than a working instance.

## Cheap Code Changes The Order Of Operations

AI changes the cost of producing and revising software.

If a system integrator has the right templates, skills, product primitives, and coding agents, they can turn customer context into a working instance much faster than before. The first version does not need to be perfect. It needs to be real enough to create useful feedback.

That changes the workflow:

```plain text
scoping -> instance -> scoping -> instance -> done
```

The key shift is that delivery can move earlier.

Instead of treating delivery as the final output of discovery, the system integrator can use delivery as part of discovery. A customer conversation can generate enough signal for a first version. The customer can then react to actual behavior, not just a description of future behavior.

The working instance becomes the alignment artifact.

## Delivery Becomes A Learning Tool

When customers react to documents, their feedback is often abstract.

They may approve a workflow on paper and then realize something feels wrong when they use it. They may sign off on a field list and later discover that a role should not see certain data. They may agree to a process diagram and then realize the approval step needs to happen earlier.

When customers react to working software, the feedback gets more concrete:

- "This is close, but the approval step should happen earlier."
- "These fields are right, but this role should not see them."
- "This dashboard is missing the metric the VP cares about."
- "This workflow is correct for the main team, but the regional teams need a variant."

That kind of feedback is more useful because it attaches to a real artifact.

The system integrator no longer has to interpret everything from abstract requirements. They can learn from the customer's reaction to something concrete.

## The Role Of The System Integrator Changes

Cheap code does not make system integrators less important.

It changes where their expertise matters.

The old model rewarded the ability to extract requirements, document them clearly, and translate them into an implementation later. The new model rewards the ability to orchestrate a fast implementation loop without letting it become chaotic.

The integrator still needs to know:

- What questions to ask.
- Which customer signals matter.
- What should be generated quickly.
- What needs deeper architectural care.
- What can remain rough for feedback.
- What needs to be locked down.
- How to keep the customer aligned while the instance changes quickly.

In other words, cheap code increases the leverage of the system integrator. It does not replace their judgment.

## Documentation Still Matters

This is not an argument against documentation. It is an argument for changing the role of documentation.

When code was expensive, documents often substituted for software. They were the thing customers reviewed because the working instance did not exist yet.

When code is cheap, documents can become supporting context around the working instance:

- What was decided.
- Why it was decided.
- Which customer signal led to a change.

Documents stop being the main substitute for software and become the memory around the implementation.

## The New Assumption

The old assumption was:

> We need to be very sure before we build, because building and changing are expensive.

The new assumption is:

> We can build earlier because changing is cheaper, and a working instance teaches us faster than another abstract scoping cycle.

That is the strategic implication of cheap code for system integrators.

It means the fastest path to alignment may no longer be more scoping before delivery.

The fastest path to alignment may be a working instance.

## The Product Question

If system integrators can work this way, they need a way to make the process visible, collaborative, and trusted.

Cheap code by itself can feel chaotic. Customers need to understand what they are reviewing. Integrators need to control what is shared. Feedback needs to attach to the right artifact. Decisions need to be remembered. Iterations need to feel like progress, not randomness.

That is the product system integrators need now: a workflow where fast software changes become visible, collaborative, and trusted. It is what we are building at Auctor.
