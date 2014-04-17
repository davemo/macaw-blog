---
title: "The SCNA 2011 Narrative"
author:
  name: "Dave Mosher"
---

I attended [Software Crafstmanship North
America](http://scna.softwarecraftsmanship.org/) in Chicago this weekend and
came away feeling much differently than I thought I would. I [tweeted a
summary](https://twitter.com/dmosher/status/138476620896931840) of my thoughts
last night:

> @dmosher: I find it interesting that the talks I agreed with most at \#scna
> were predominantly against established "agile" principles … :|

Twitter is a horrible medium for expressing ideas that are packed with meaning;
this post is intended to unpack my tweet and experience at SCNA 2011 by focusing
on the 3 talks I found the most valuable and how they formed a cohesive and
powerful narrative in my mind.

## Suitability vs Capability

[Gary Bernhardt](http://twitter.com/#!/garybernhardt) gave a wonderful talk
entitled "Expansion & Contraction". I think he should have titled it
"Suitability vs Capability" but it was a brilliant talk and the one I considered
the best of the conference. Here's my best attempt at paraphrasing it:

> Programming Language and Technology go through a constant ebb and flow of
> expanding and contracting over time. During expansion, these solutions are
> "Capability" solutions; that is, they are capable of solving problems but they
> are not yet suitable. Eventually there is a contraction that happens and
> "Suitability" solutions emerge.
>
> Java first emerged as a Capability Solution during an expansion in the post
> C/C++ era. Time passed and a contraction occurred in which Java matured into a
> Suitability Solution for developing software.

A few times during his talk Gary mentioned that JavaScript and NodeJS are
currently in the realm of Capability Solutions. At first this rubbed me the
wrong way but I think that's because I wasn't really listening to what he was
saying *objectively*. NodeJS is absolutely in the realm of Capability and not
Suitability at the moment, but that doesn't mean you can't create something
useful with it.

Thinking more about the heart of Gary's talk I find myself glad that it was on
Day 1 because I found that it framed my thinking for the rest of the conference.

## Programmer Anarchy

Agile best practices are often framed as things we "must do" in order to be
successful but I think it would behoove us to frame them in terms of suitability
and capability.

[Fred George](http://twitter.com/#!/fgeorge52) gave a talk in the breakout room
on Day 2 entitled "[Programmer
Anarchy](http://forwardtechnology.co.uk/videos/32447325)". His ideas might seem
radical to some but I think they are an appropriate response based on an
evaluation of suitability/capability for his *specific situation*. It's
important to understand that the following decisions derive from a company that
is continually investing in new ways to make money by building very small
applications. Here's the gist:

> Agile prescribes many best practices like Kanban, Scrum, XP, Pairing,
> Continuous Integration, Unit Testing... the list goes on.
>
> In the waterfall era the power to determine *how* systems get built lies
> squarely with the *customer*. Up-front design docs and requirements
> specifications dictate how developers should build a system to achieve
> success. Through waterfall, systems are often built completely wrong. As a
> result customer trust is lower, developer happiness decreases, and success is
> not realized.
>
> In the agile era the power to determine *how* systems get built is *shared*
> between the *customer and developers* but there is a gap in trust because of
> the past failures of waterfall. Agile is an attempt to bridge the trust gap by
> building things faster and with less bugs. Through agile, systems are also
> built wrong but they fail faster which mitigates risk and decreases the cost
> of change.
>
> In the era of Programmer Anarchy the power to determine *how* systems are
> built lie directly with *developers.*
>
> -   non-developer roles like architects, project manager, scrum-master, team
>     lead, delivery lead, hr people and tester are completely eliminated from
>     teams
> -   developers are empowered to build software using whatever technology they
>     choose and with whatever tools they choose
> -   applications and systems are extremely small (100-300 lines of code) so
>     unit-tests, acceptance tests, and continuous integration are eliminated
>     entirely
> -   teams are encouraged to write and re-write applications using whatever
>     they want, including capability solutions (Clojure, NodeJS, Cassandra,
>     Hadoop, etc..)

Fred talked a lot about his company and how they have a lot of trust in their
developers to be able to turn ideas into money. The first thing they do on any
project is write the business metrics code to be able to verify whether
something they produce can be tied back to business value. This is an absolutely
*critical point* that needs to be understood. Most of the time, my
dissatisfaction in the work I do is related to not knowing whether something I
build will *actually* have value. If I had metric and monitoring code in place
that was able to tell me what I created is making money and can be considered
successful my job satisfaction would increase greatly.

Unit tests weren't suitable for Fred's teams because they were writing such
small applications, so they eliminated them. Traditional "Agile" roles weren't
suitable because he empowered developers to make decisions on what to use, how
to use it and which developers would be best suited to building it, so they
eliminated them. I think you can see the pattern.

I found it interesting that Fred's teams got rid of things many in the Agile
movement consider to be not only suitable but *essential* to building good
software. It was also fascinating that he actively pushed his teams to use
capability solutions like Clojure, NodeJS, Cassandra and Hadoop, which proved
wildly successful.

Whether you agree with the decisions or not is irrelevant; Fred's team made a
judgement call about the suitability of all the typical "Agile" best practices
and cut away all the things that weren't suitable. Good teams find ways to
eliminate waste by evaluating whether the things they do are capable *and*
suitable and eliminating things that aren't.

## Propaganda, Indoctrination, Fanbois, and Education

I believe there to be a significant difference between a "Big 'A' Agile" and
"Little 'a' agile". The religion of "Agile" is often touted as the one single
way to build software. The number of roles and processes prescribed by "Agile"
is excessive, however, this is due to a failure to evaluate things in terms of
whether they are suitability solutions or capability solutions for a given
project/team.

It was probably surprising to people in the software craftsmanship movement that
[Zed Shaw](http://twitter.com/zedshaw) was invited to speak, but his talk on
"Propaganda, Indoctrination, Fanbois, and Education" was the most thought
provoking talk at SCNA 2011. Here's my translation:

> Anyone who tells you that they have found the "one true way" to build software
> is a con-artist trying to sell you something.
>
> If you aren't writing code, you aren't a programmer. Programmers build
> software, everything else is just marketing spin.
>
> Indoctrination happens when you're convinced to think something is the only
> way. Education gives you options and lets you make choices. Don't be
> indoctrinated, be educated.
>
> Agile and all the related buzzwordy ideas can be boiled down to these 3 simple
> ideas:
>
> -   Make a list of stuff to do.
> -   Do that stuff.
> -   Automate the heck out of everything.
>
> (note: these things don't have to be done in any particular order)

While he's abrasive and rubs a lot of people the wrong way, Zed Shaw has done a
lot of good for the software craftsmanship movement. He's trying to put the
focus back on learning programming instead of "Super XP Double Pairing Kanban
Scrum Sauce" and all the rest of the "Agile" marketing spin. His ["Learn Code
the Hard Way"](http://learncodethehardway.org/) series is wildly successful and
is actually teaching people how to program. Somebody at the conference asked
him:

> "So what do you think about Unit Testing and Continuous Integration and all
> that stuff then?"

His response was pretty down to earth:

> I've worked for big consulting companies doing every one of those things in
> the past. I've written tests, done TDD, used pivotal tracker blah-de-bloo or
> whatever you're using. Those things aren't bad but anyone who is trying to
> tell you those things are the "one true way" to build software is a con-artist
> trying to sell you something. If you believe that stuff you've got a
> mind-virus. You don't want a mind-virus.

I used to change my thinking *drastically* all the time. I'd go to conferences
and experience a lot of hype and get infected with a mind-virus that led me to
adopt ideas that I would later on discard. This isn't a healthy thing to do.
Nothing I experienced at SCNA 2011 was radical enough to make me change my
thinking drastically, but what I did experience will help me to be much more
objective about the things I let influence me going forward.

## Where do we go from here?

It's important to be objective. It's important to question the value of things
we do, especially when we do them because somebody has told us they will solve
all our problems.

To me, the most important narrative of SCNA 2011, and the thoughts behind my
[tweet](https://twitter.com/dmosher/status/138476620896931840) are these:

-   Don't buy into all the propaganda, don't get indoctrinated. Get educated.
-   Learn to *objectively* evaluate the tools, processes, and ideas we use in
    terms of *suitability and capability*.
-   Let go of suitability solutions if they don't give you any value.
-   Embrace capability solutions because you might be surprised by their value.
