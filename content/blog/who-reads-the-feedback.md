+++
title = "Who Reads The Feedback"
date = "2026-10-22"
description = "When agents do the work, feedback meant for people never reaches them. The time I used to spend teaching authors now goes into teaching agents."
tags = ["ai", "software", "learning"]
+++

For most of software history, code review was also teaching. A senior engineer left comments on a pull request, the author read them and fixed the code, and the author remembered the lesson the next time. The feedback improved one change and made the person who wrote it better at their job.

That loop is breaking. When I review frontend work now, I leave comments about a component that should be reused or state that belongs in a different place. The author doesn't read them. They point their coding agent at the comments, the agent makes the changes, and the pull request gets approved. The code gets better, but the author learns nothing, because the author never read the feedback.

The only thing my comment taught was the agent, and only for that one pull request. The agent doesn't remember it. Next week a different author's agent makes the same mistake, and I leave the same comment again.

That is why it feels like it's not worth teaching anyone anything anymore. Teaching a person pays off only if that person does the work next time. When an agent does the work, the lesson has to go to the agent.

So I've started spending my review time differently. When I see the same frontend mistake twice, I write it into an agent skill instead of a PR comment. A skill is a set of written instructions the agent loads before it starts working. Once a rule is in the skill, every agent that loads it follows that rule on every pull request, no matter who the author is. One edit to the skill replaces a comment I would otherwise write fifty times.

This is closer to writing a style guide than to mentoring. The difference is that the reader actually follows every line.

Right now this mostly applies to software engineering, because coding agents are the most capable agents we have. It won't stay that way. As agents start drafting contracts and building financial models, the same thing will happen in law and finance. A partner will mark up a junior's contract, the junior's agent will make the edits, and the junior will approve the result without reading the markup.

That leaves a question I can't answer yet. If people stop learning from feedback, how does anyone get experienced enough to give it? The people writing skills today built their judgment by having their own work corrected. I don't know what replaces that.

For now, I put my review time into skills. A PR comment changes one pull request. A change to a skill changes every pull request after it.
