# How to use silos effectively

There are as many models for organizing teams around functionality as there are
systems for managing project work. There is no point in getting religion around
organizational structure like silos vs full-stack vs cross-functional teams the 
way one might have religion around vi vs emacs, because just like vi and emacs, 
or Mac vs Windows, or any X vs any Y, every tool has its strong and weak points, 
and your job is to choose the right tool at the right time to do the work that you have.

The advantage of a silo is that you concentrate subject matter knowledge in a team
so that everyone on the team is good and gets better in that problem space. With 
all your DBAs in one team,
talking together, everyone knows who can help them when they get stuck, and people
can easily collaborate or share ideas. The shared context eliminates the overhead 
of having to explain concepts or establish baseline understandings. Everyone here
knows what a transaction is and what a rollback means; we know what a replay is. 
Everyone on your networking team, from the most junior person to the CCIE, knows
the difference between layers 3 and 4. You can hit the ground running, people
can hand tasks off easily, and you can always rely on someone to back you up 
when you get stuck.

The disadvantage of a silo, and why many organizations have moved to 
cross-functional teams, is that ... it concentrates subject matter knowledge
in one team. Your software developers write unoptimized queries because they 
don't know database internals. The network team runs frontend load balancers 
that brown out your service sometimes because they won't configure custom health 
checks per service and apply a one-size-fits-all approach that's easiest for
them to manage. Every time you need to involve another team, you need to 
have a meeting and write justifications.
Pretty soon, everything is just a hopeless pile of workarounds that don't
really work.

Melvin Conway is quoted as saying, "any organization that designs a system 
(defined broadly) will produce a design whose structure is a copy of the 
organization's communication structure." This is known as Conway's Law, and in
the context of tech organizations it means that your product's architecture 
will mirror your organization's team structure. Frontend coders will write
a frontend that talks to the APIs on the backend; the backend server will
start spinning up duplicative caches because the database is slow and then everything will
be answered by "eventual consistency"; the network will be a black box that people
document in Excel worksheets and just hope for the best from; and the devops team 
will disable the light bulbs in their area and start to speak only in 
sentences that start with "I told them that--." 

Knowing that the product will take on the aspect of the organization, your
challenge as a leader is to stop thinking about team organiations from the
business' perspective and think about it from the product's perspective. What does
your product or service do? Who are its users? Where are the logical breakpoints
between given functional areas of the product, and how do you arrange a team with
the right set of skills in a team to support each area? 

Planning the organizational structure from the product perspective may still mean
that you wind up with silos, to a certain extent. Maybe all your DBAs are still
clustered together, but now they're on the backend team working with the people
writing the APIs; everyone understands what the data is and how the APIs are
called to retrieve it, so the DBAs can figure out the
right way to structure the data so queries are fast, and now the backend team 
doesn't need to add layers of caching that introduce points of failure. 

In the end, the tl;dr of how to use silos appropriately is the same story we
had in the beginning. Build a silo where a silo will help,
and tear it down when it's a hindrance. Knowing that your product will mirror your
organization, start from the product and work backwards to build the organization.


# For additional reading

* Tune, N. (2018, May 11). An Introduction to Sociotechnical Architecture Patterns. Retrieved from https://medium.com/nick-tune-tech-strategy-blog/an-introduction-to-sociotechnical-architecture-patterns-ea64a75c2aaf
* Tune, N. (2019, September 25). Organisational Dysfunctions Mirrored as Architectural Complexity. Retrieved from https://medium.com/nick-tune-tech-strategy-blog/organisational-dysfunctions-mirrored-as-architectural-complexity-b5a903b3f5b2

