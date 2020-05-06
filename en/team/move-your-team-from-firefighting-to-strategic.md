# How to move your team from firefighting to strategic

Depending on the sort of team you're managing, they may be susceptible to being stuck in 
a firefighting mode, constantly stuck dealing with an issue that's on fire right now but
never able to make the changes to fix the problem in the long-term because something
somewhere is always on fire. This is a hard situation to turn around, but it's common and
can be done.

When you're in a crisis, the first thing to do is to triage. Triage means to assess
problems, sort them by criticality, and then do what you can to fix the things that can
be fixed. Not everything is actually critical, and not everything can be fixed. Be
honest and pragmatic, and don't panic.

In an outage situation, triage can be a fast process. Suppose you lost a database 
index and now the product catalog is broken on the public-facing website. Your choices are to
fix the catalog by rebuilding the index, or by restoring from backup. Assess: How can you
rebuild the index, how long will it take, and will rebuilding that index cause anything
else to fail? How long would it take to restore from a backup, and how much data would you 
lose from the interim time between now and that backup? Once you understand the 
implications of your options, you can choose a course of action, communicate it, and act
on it.

But in daily situations, someone may just take "this is how it is" for granted and not
even engage in triage at all. They might work on the issue that they're being paged for,
without looking at other issues and realizing that there's a more important ticket about
the root cause. This situation is a sort of alarm fatigue, where there are so many things
yelling at you that you don't really even notice them anymore.

So your challenge as the manager of a team which is caught in the firefighting cycle
is first to recognize that you are caught, to triage the problems, and then to 
use your judgment of priority to split your team's energies between fixing the 
truly critical live problems and fixing the root causes. Plans or processes will be a 
help; the less time you have to spend figuring out how to deep-dive a root cause 
analysis on each new problem, the more time you have to actually solve the root cause. Don't 
attempt to solve everything up front, either: start with a simple, short, and generic
template, and iterate your procecss over time as you learn what's important to your
team and organization. Step in and direct the team's 
efforts as much as practical to reducing the sources of failure, like a fire captain
who sets some firefighting teams to stopping houses from catching fire from flying
embers and some to putting out the source, but get out of the way and let them do
their jobs when they don't need your help.

As you gradually handle the root causes of your fires, make sure to recognize the 
emotional effects on your team. A very long-standing firefighting situation may cause
engineers to become burned out, risk-averse, disengaged, or to feel hopeless. Ask 
them how they are doing and how they feel about the work they're doing, actively listen 
to their concerns, and show empathy for them. Recognize where they are down, but also
show them their progress over time;
that's especially important when the progress is less obvious and people might be
going home every day with a feeling that they didn't actually "do" anything, like
when the change is slow or hidden, like a slowed rate of incoming tickets, or only 
three customer-impacting events a week instead of four. 

And tell people to take their vacations, and turn off their pagers. 
