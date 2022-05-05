# 1. What is Software Engineering?

We see three critical differences between programming and software engineering: time, 
scale and the trade-offs at play.
On a software engineering project, engineers need to be more concerned with the passage
of time and the eventual need for change.
In a software engineering organization, we need to be more concerned about scale and 
efficiency, both for the software we produce as well as for the organization that is 
producing it.
Finally, as software engineers, we are asked to make more complex decisions with 
higher-stakes outcomes, often based on imprecise estimates of time and growth. 

Within Google, we say, "Software engineering is programming integrated over time". 
We might need to delineate between programming tasks (development) and software
engineering tasks (development, modification, maintenance). The addition of time 
adds an important new dimension to programming. 

One way to see the impact of time on a program is to think about the question, 
"What is the expected life span of your code?" It is just as reasonable to think
of code that needs to last for a few minutes as it is to imagine code that will live
for decades. Short-lived systems are effectively "just" a programming problem.
As we expand that time to allow for longer life spans, change becomes more important.
Over a span of a decade or more, most program dependencies, whether implicit or 
explicit, will likely change. This recognition is at the root of our distinction 
between software engineering and programming.

This distinction is at the core of what we call *sustainability* for software.
Your project is *sustainable* if, for the expected life span of your software, 
your are capable of reacting to whatever valuable change comes along, for either
technical or business reasons.

Another way to look at software engineering is to consider scale. How many people
are involved? What part do they play in the development and maintenance over time?
A programming task is often an act of individual creation, but software engineering
task is a team effort. Team collaboration presents new problems, but also provides
more potential to produce valuable systems than any single programmer could.

Team organization, project composition, and the policies and practices of a software
project all dominate this aspect of software engineering complexity. These problems
are inherent to scale: as the organization grows and its projects expand, does it 
become more efficient at producing software? Does our development workflow become 
more efficient as we grow, or do our version control policies and testing strategies
cost us proportionally more?

We can also say that software engineering is different from programming in terms of 
the complexity of decisions that need to be made and their stakes. The job of a 
software engineer, or a software engineering leader, is to aim for sustainability 
and management of the scaling costs for the organization, the product and the 
development workflow. With those inputs in mind, evaluate your trade-offs and make 
rational decisions. 

## Conclusion
We believe it is important to differentiate between the related-but-distinct terms 
"programming" and "software engineering". Much of that difference stems from the 
management of code over time, the impact of time on scale, and decision making in 
the face of those ideas. Programming is the immediate act of producing code. 
Software engineering is the set of policies, practices and tools that are necessary
to make that code useful for as long as it needs to be used and allowing collaboration
across a team.