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

### Pace of Progress
Here's another analogy. Think about how you work with your compiler. When you sit 
down to write a large piece of software, do you spend days writing 10,000 lines of
code, and then, after writing that final, perfect line, press the "compile" button
for the very first time? Of course you don't. Can you imagine what sort of disaster
would result? Programmers work best in tight feedback loops: write a new function,
compile. Add a test, compile. Refactor some code, compile. This way, we discover 
and fix typos and bugs as soon as possible after generating code.
This is how we keep code quality high and make sure our software is evolving 
correctly, bit by bit. The current DevOps philosophy toward tech productivity is 
explicit about these sorts of goals: get feedback as early as possible, test as 
early as possible, and think about security and production environments as early 
as possible. This is all bundled into the idea of "shifting left" in the developer
workflow; the earlier we find a problem, the cheaper it is to fix it.


The same sort of rapid feedback loop is needed not just at the code level, but at 
the whole-project level, too. Ambitious projects evolve quickly and must adapt to 
changing environments as they go. How do you get that feedback loop so that you 
know the instant your plans or designs need to change? Answer: by working in a team.

### In Short, Don't Hide
So, what "hiding" boils down to is this: working alone is inherently riskier than 
working with others. Even though you might be afraid of someone stealing your idea 
or thinking you're not intelligent, you should be much more concerned about wasting 
huge swaths of your time toiling away on the wrong thing.

## It's All About the Team

The point we’ve been hammering away at is that, in the realm of programming, lone
craftspeople are extremely rare—and even when they do exist, they don’t perform
superhuman achievements in a vacuum; their world-changing accomplishment is
almost always the result of a spark of inspiration followed by a heroic team effort.
A great team makes brilliant use of its superstars, but the whole is always greater than
the sum of its parts. But creating a superstar team is fiendishly difficult.
Let’s put this idea into simpler words: *software engineering is a team endeavor*.

This concept directly contradicts the inner Genius Programmer fantasy so many of us
hold, but it’s not enough to be brilliant when you’re alone in your hacker’s lair. 
You’re not going to change the world or delight millions of computer users by hiding 
and preparing your secret invention. You need to work with other people. 
Share your vision. Divide the labor. Learn from others. Create a brilliant team.

### The Three Pillars of Social Interaction
So, if teamwork is the best route to producing great software, how does one build (or
find) a great team?
To reach collaborative nirvana, you first need to learn and embrace what I call the
“three pillars” of social skills.
+ *Pillar 1: Humility*
You are not the center of the universe (nor is your code!). You’re neither 
omniscient nor infallible. You’re open to self-improvement.
+ *Pillar 2: Respect*
You genuinely care about others you work with. You treat them kindly and
appreciate their abilities and accomplishments.
+ *Pillar 3: Trust*
You believe others are competent and will do the right thing, and you’re OK with
letting them drive when appropriate

If you perform a root-cause analysis on almost any social conflict, you can ultimately
trace it back to a lack of humility, respect, and/or trust.

### Humility, Respect, and Trust in Practice

#### Lose the ego
Nobody wants to work with someone who consistently behaves like
they’re the most important person in the room. Even if you know you’re the wisest
person in the discussion, don’t wave it in people’s faces.

Although it’s important to be humble, that doesn’t mean you need to be a doormat;
there’s nothing wrong with self-confidence. Just don’t come off like a know-it-all.

#### Learn to give and take criticism
In a professional software engineering environment, criticism is almost never personal—
it’s usually just part of the process of making a better project. The trick is to
make sure you (and those around you) understand the difference between a constructive
criticism of someone’s creative output and a flat-out assault against someone’s
character.
On the other side of the conversation, you need to learn to accept criticism as well.
This means not just being humble about your skills, but trusting that the other person
has your best interests (and those of your project!) at heart and doesn’t actually think
you’re an idiot. Programming is a skill like anything else: it improves with practice. If
a peer pointed out ways in which you could improve your juggling, would you take it
as an attack on your character and value as a human being? We hope not. In the same
way, your self-worth shouldn’t be connected to the code you write—or any creative
project you build. To repeat ourselves: *you are not your code*. Say that over and over.
You are not what you make. You need to not only believe it yourself, but get your
coworkers to believe it, too

### Blameless Post-Mortem Culture
The key to learning from your mistakes is to document your failures by performing a
root-cause analysis and writing up a *postmortem*. Take extra care to make sure the 
postmortem document isn’t just a useless list of apologies or excuses or 
finger-pointing—that’s not its purpose. A proper postmortem should always contain 
an explanation of what was learned and what is going to change as a result of the 
learning experience. Then, make sure that the postmortem is readily accessible and 
that the team really follows through on the proposed changes.
A good postmortem should include the following:
+ A brief summary of the event
+ A timeline of the event, from discovery through investigation to resolution
+ The primary cause of the event
+ Impact and damage assessment
+ A set of action items (with owners) to fix the problem immediately
+ A set of action items to prevent the event from happening again
+ Lessons learned

## Conclusion
The foundation for almost any software endeavor—of almost any size—is a wellfunctioning
team. Although the Genius Myth of the solo software developer still persists,
the truth is that no one really goes it alone. For a software organization to stand
the test of time, it must have a healthy culture, rooted in humility, trust, and respect
that revolves around the team, rather than the individual. Further, the creative nature
of software development requires that people take risks and occasionally fail; for people
to accept that failure, a healthy team environment must exist.

# 3. Knowledge Sharing
Your organization understands your problem domain better than some random person
on the internet; your organization should be able to answer most of its own questions.
To achieve that, you need both experts who know the answers to those
questions and mechanisms to distribute their knowledge, which is what we’ll explore
in this chapter. These mechanisms range from the utterly simple (Ask questions;
Write down what you know) to the much more structured, such as tutorials and
classes. Most importantly, however, your organization needs a *culture of learning*, 
and that requires creating the psychological safety that permits people to admit 
to a lack of knowledge.

## Challenges to Learning
Sharing expertise across an organization is not an easy task. Without a strong 
culture of learning, challenges can emerge. Google has experienced a number of 
these challenges, especially as the company has scaled:

+ *Lack of psychological safety*
An environment in which people are afraid to take risks or make mistakes in
front of others because they fear being punished for it. This often manifests as
a culture of fear or a tendency to avoid transparency.

+ *Information islands*
Knowledge fragmentation that occurs in different parts of an organization that
don’t communicate with one another or use shared resources. In such an 
environment, each group develops its own way of doing things. This often leads
to the following:
..+ *Information fragmentation*
..Each island has an incomplete picture of the bigger whole.
..+ *Information duplication*
..Each island has reinvented its own way of doing something.
..+ *Information skew* 
..Each island has its own ways of doing the same thing, and these might or
..might not conflict.