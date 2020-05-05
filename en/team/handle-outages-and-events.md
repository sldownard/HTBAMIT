# How to handle outages and events

Don't Panic.

If you were an engineer before you became an engineering manager, then you've been through
this before: you get a page, your heart sinks to the floor, you get online and start looking
at the logs, trying to see what's gone wrong so you can fix it. 

A lot of what you should do in an outage will depend on what your team does and what customers
you serve. If you are keeping a retailer's POS terminals online, the specifics of what you do
in an event will vary from someone who is keeping a CDN node available. But in general, the
things you need to do are:

1. Assess the problem.
1. Fix the problem.
1. Communicate about the problem.
1. Remediate the problem.

And definitely: Don't Panic. You set the tone for your engineers, and they will take
their cues from you. If you are angry, or upset, they will become angry and upset. But
if you calmly assess the situation, and coolly handle the communications, you will
make the situation less stressful and people will trust that things are under control.

As the team manager, resist the urge to meddle with your engineers; adding the 
distraction of having to manage you, while they are already trying to manage a
complex technical problem will add overhead and may slow down the resolution. You
want to remove blockers, not add them, so unless they specifically come to you 
for help, or if someone is struggling or wavering about what to do, let them be
the technical experts on the ground. You are Mission Control, and your job during 
the event is to communicate about the problem to stakeholders,
customer service and support, and dependencies/interested parties. After the event, 
your job is to debrief with the team, analyze the event, and correct the conditions 
that led to the outage.

Because you are Mission Control and not the astronauts, you might feel unsettled,
or feel like you should be on the ground actually solving the problem. You need to
resist that, and stay focused on getting information where it needs to go. Be the
hands writing notes for your team so they don't need to, be the record of what has
happened for when they are stressed and can't remember what happened when they tried
an idea. Get customer support the updates they need for your customers, and give
your stakeholders the updates they require, and be there for your engineers to
help them be effective. This is your contribution during the event.

Hopefully your organization has a plan for major events, but if you work for a smaller
organization, or a newer one, you might need to create one. You should do this before
one happens. A great way to do that is to do game days: an exercise where you
break something in a non-production environment and practice recovering it using your
existing operational tools and runbooks. It's important to treat it as if it were prod 
and not take shortcuts (for example, actually write an update and try to post it to
the non-prod version of your customer-facing status page,
don't just say "next, I would post to the status page") so that you actually use 
the same tools and processes that you would during a real event. Just like an
uncommon code path, you won't know what your tests don't cover until you exercise it.

After the event, keep your cool. You must resist at all costs the urge to point
fingers. What about if it wasn't your team's fault, but a service you depend on had
an outage that cascaded to cause your issue?
Analyze your use of that dependency, and see if there are things you could do 
differently. If there are, you can see if they are worth pursuing, and if there aren't,
you need to choose if you accept the risk or if you should get off that dependency.
This is the information you can take back to the business to resolve any lingering
dissatisfaction after the event.


# Additional reading
* Amazon Web Services. (n.d.). AWS Well-Architected Framework: Concepts: Game Day. Retrieved April 27, 2020, from https://wa.aws.amazon.com/wat.concept.gameday.en.html
  - This page goes over AWS' process for running a game day to test failures and processes, 
    how to analyze the results, and to use a correction of error process to resolve the 
    issues that came up during the game day.

