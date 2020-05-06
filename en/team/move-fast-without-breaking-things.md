# How to move fast without breaking things

Facebook adopted the motto "move fast and break things" as a way of encouraging
teams to minimize risk aversion, and to enable them to challenge the status quo and 
innovate rather than playing it safe. But in 2014, even they backed down from breakage, 
and changed it to "move fast with stable infrastructure." It turns out that
customers don't like it when we move so fast we break their stuff.

The challenge that we have as technical managers is to enable our teams to move
as quickly as possible without compromising operational stability, because ops is what we
are here for, even if you're on a team of coders that is nowhere near customer support. 
This means that you need to know what is blocking your engineers, and act to unblock them; 
you need your deployment pipeline to have enough built-in safeties, like full-stack 
integration tests with automated deployment approvals and rollbacks on bad metrics, so your 
engineers can develop and push without then having to choose between hours of manual 
tests or letting defects escape; and you need to know what's at stake with a given
project so you can tell when to hold your ground and when you can drop things when 
people tell you to get something done faster. Which they will.

In short, it comes down to three things: 
1. Quality must be a first-class citizen in your 
development process, from code reviews and unit and integ testing, to metrics and alarming, to regularly
reviewing your change process and [technical debt](address-technical-debt.md) backlogs
so you know what your operational risks are. Unless you are producing quality work,
and your automation and instrumentation can back you up on it, you will break things.
1. Understand the approach that your team has chosen to accomplish a task. Know the
safeties that you are including and how that benefits the customer more than the alternative, 
so that you can get your stakeholders' agreement that it is the right decision to include a
given task in a project. Know the difference between the must-haves and the nice-to-haves,
so you can make compromises when a compromise is appropriate.
1. Communicate. Talk to your engineers, talk to your stakeholders. If you are a black
box that information goes into to die, then your team will not be able to succeed, and 
you will be the one breaking things.

# Additional reading

* Baer, D. (2014, May 2). Mark Zuckerberg Explains Why Facebook Doesn't 'Move Fast And Break Things' Anymore. Retrieved from https://www.businessinsider.com/mark-zuckerberg-on-facebooks-new-motto-2014-5

