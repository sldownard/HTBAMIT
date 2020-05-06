# How to address technical debt

Your team will acquire technical debt. There is never enough time or effort to fix all the problems,
so building up your backlog of "we should fix this someday" tasks is unavoidable. Technical debt 
generally represents a tradeoff that was made, a calculated risk that was taken: we will 
mitigate X instead of Y, because Y is unlikely and might not occur.
We will push the feature without docs, because anyone can read the source to figure
out how it works. We will write unit tests but not block the release on additional integ 
testing because it's a very small function that will only interact with one thing.

The trouble is that those trade-off decisions are infrequently revisited. Consequently, 
one problem of tech debt is that sometimes, your risk becomes a reality. Your
API grew in scope until it was implicated in customer-facing workflows and now your 
lack of integ testing means a defect escaped and your customers' orders are being 
blackholed, and no one noticed because you didn't have anything to tell you your rate 
of incoming orders dropped to 0. 

But a second problem is just that tech debt is, like credit card debt, depressing to 
look at and to think about. Engineers can feel tech debt as a sort of failure: we 
didn't do a good job, because we left part of the work undone. We cut corners. And 
someday it's going to hurt us.

From the perspective of a manager who is in charge of a product roadmap as well as people,
you have to solve both of those problems. You need to use your limited engineering hours
to focus on doing the things that are the most important, and you need to revisit your
decisions to pay off the important debt and to preserve people's good morale (and feeling
of safety) about their environment.

One way that you can do this is to have a transparent process for gauging which operational
risks your team will accept, and which you will not. What risks are sufficiently emergent 
that you will pull them off the backlog and put them above feature development? These will
likely take the shape of risks that affect your ability to detect underlying problems: 
do you have alarms, do your alarms fire on the right criteria, do you automate rotating your
SSL certificate prior to its expiration, are you able to trace a 
single customer request-id across six or ten different microservices, from browser
to billing records, without having to build an architectural diagram to do it? Build a list
of what things you will consider "important," and go down the backlog with the entire team
sorting them into low/medium/high. Ask the team what worries they have, that keep them from
sleeping easy (or from being willing to take a long vacation), that aren't on the backlog?
Make this a process, and do it on a schedule, so that your backlog of debt doesn't simply
grow indefinitely.

When you have a triaged list of tasks from the backlog, talk about what the next steps
are, and be transparent about what risks you may have to accept because of your resources.
Remember the pareto principle, which says 80% of the effects come from 20% of the causes;
that means 80% of the risk is from 20% of your backlog, or to put it positively, 80% of
the benefit comes from completing 20% of the work. Pick your 20% wisely.

Discard the tasks that you know you are not going to do. Move them to a wont-fix backlog to 
keep the knowledge in case it's ever needed, mark them resolved and archive them, or do
something else, but but get them out of sight. A list of things you will not do 
is not useful, and it will just leave bad feelings, like a room in a house that's 
full of junk, so you avoid going into it and can't get anything useful from. A backlog 
of noise is garbage and it will make your team feel bad. Throw it away.

When you and your team regularly assess your technical debt, discard the things that you
all agree are not important, and whittle away those things that are, people will feel
like they are spending their time on the right work, making good progress, and 
like the team's work product is balanced and healthy. 

