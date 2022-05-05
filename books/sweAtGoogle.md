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

# 2. How to Work Well on Teams

The critical idea in this chapter is that software development is a team endeavor. 
And to succeed on an engineering team you need to reorganize your behaviors around
the core principles of humility, respect and trust.

## The Genius Myth
Many humans have the instinct to find and worship idols. For software engineers,
those might be Linus Torvalds or Bill Gates- all heroes who changed the world with
heroic feats. Linus Torvalds wrote Linux  by himself, right? 

Actually, what Linus did was write just the beginning of a proof-of-concept 
Unix-like kernel and show it to an email list. Linux is hundreds of times bigger
than that initial kernel and was developed by *thousands* of smart people. Linus's 
real achievement was to lead these people and coordinate their work; Linux is the 
shining result not of his original idea, but of the collective labor of the community.

The Genius Myth is the tendency that we as humans need to ascribe the success 
of a team to a single person/leader. Humans have a natural instinct to find leaders
and role models, idolize them, and attempt to imitate them. We all need heroes for 
inspiration, and the programming world has its heroes, too.

But even if you are a genius, it turns out that that's not enough. Geniuses still
make mistakes, and having brilliant ideas and elite programming skills doesn't 
guarantee that your software will be a hit. Worse, you might find yourself solving
only analytical problems and not *human* problems. Being a genius is most definitely
not an excuse for being a jerk: anyone - genius or not - with poor social skills 
tends to be a poor teammate. The vast majority of the work at Google doesn't require
genius-level intellect, but 100% of the work requires a minimal level of social 
skills. What will make or break your career is how well you collaborate with others.

## Hiding Considered Harmful
If you spend all of your time working alone, you're increasing the risk of unnecessary
failure and cheating your potential for growth. 

First of all, how do you even know whether you're on the right track?

### Early Detection
If you keep your great idea hidden from the world and refuse to show anyone 
anything until the implementation is polished, you're taking a huge gamble. It's 
easy to make fundamental design mistakes early on. You risk reinventing wheels.
You need to make sure that you're working on the right thing, you're doing it 
correctly, and it hasn't been done before.

Early sharing isn't just about preventing personal missteps and getting your ideas 
vetted. It's also important to strengthen what we call the bus factor of your project.

### The Bus Factor
*the number of people that need to get hit by a bus before your project is completely doomed*
How dispersed is the knowledge and know-how in your project? If you're the only 
person who understands how the prototype code works, you might enjoy good job 
security- but if you get hit by a bus, the project is toast. If you have a small 
team designing and prototyping together, things are better- the project won't be 
marooned when a team member disappears. Ensuring that there is *at least* good 
documentation in addition to a primary and a secondary owner for each area of 
responsability helps future-proof your project's success and increases your project's 
bus factor. Hopefully most engineers recognize that it is better to be one part 
of a successful project than the critical part of a failed project.

Beyond the bus factor, there's the issue of overall pace of progress. It's easy to 
forget that working alone is often a tough slog, much slower than people want to
admit. Working with other people directly increases the collective wisdom behind 
the effort. Programming is hard. Software engineering is even harder. You need 
that second pair of eyes.

