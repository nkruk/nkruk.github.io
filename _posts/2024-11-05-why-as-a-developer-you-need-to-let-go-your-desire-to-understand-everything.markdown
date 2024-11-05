---
layout: post
title:  "Why as as developer you need to let go of your desire to understand everything"
date:   2024-11-05 20:45:22 +0100s
---

I recently picked up a Math textbook after 20 years, and I've been going through it since August. I learned subjects that I do not recollect having studied in secondary school. My first impression was: "kind of makes sense almost nobody likes this." You are given some formulas without context, like the 'binomial theorem' and you are given some material to apply it. "This is what an LLM does", was my second thought. A mindless puzzle. "Here are a few patterns for you, turn this input into an output." Is Math simply the brain's gym? (And that line only makes sense, if you are like me and you rather watch paint dry than hitting the gym).

Then I found an amazing article online "A Mathematician's Lament" by Paul Lockhart. A little bit after explaining how "A mathematician, like a painter or poet, is a maker of patterns", he concludes:
> This is why it is so heartbreaking to see what is being done to mathematics in school. This rich and fascinating adventure of the imagination has been reduced to a sterile set of “facts” to be memorized and procedures to be followed.  

> The area of a triangle is equal to one-half its base times its height.” Students are asked to memorize this formula and then “apply” it over and over in the “exercises.” Gone is the thrill, the joy, even the pain and frustration of the creative act. There is not even a problem anymore. The question has been asked and answered at the same time— there is nothing left for the student to do.

And finally:
> The main problem with school mathematics is that there are no problems. Oh, I know what passes for problems in math classes, these insipid “exercises.” “Here is a type of problem. Here is how to solve it. Yes it will be on the test. Do exercises 1-35 odd for homework.” What a sad way to learn mathematics: to be a trained chimpanzee.  

> The point is you don’t start with definitions, you start with problems. Nobody ever had an idea of a number being “irrational” until Pythagoras attempted to measure the diagonal of a square and discovered that it could not be represented as a fraction. Definitions make sense when a point is reached in your argument which makes the distinction necessary. To make definitions without motivation is more likely to cause confusion.  

> We learn things because they interest us now, not because they might be useful later. But this is exactly what we are asking children to do with math.  

Lockhart proposes instead of the canonical way of teaching Math to children the following ideas:
> Play games! Teach them Chess and Go, Hex and Backgammon, Sprouts and Nim, whatever. Make up a game. Do puzzles. Expose them to situations where deductive reasoning is necessary. Don’t worry about notation and technique, help them to become active and creative mathematical thinkers.

He caps it up with a fictional platonic dialog between an sceptic and a believer of his proposal:
> Simplicio: So we’re supposed to just set off on some free-form mathematical excursion, and the students will learn whatever they happen to learn?  

> Salviati: Precisely. Problems will lead to other problems, technique will be developed as it becomes necessary, and new topics will arise naturally. And if some issue never happens to come up in thirteen years of schooling, how interesting or important could it be?  

> Simplicio: But then how can schools guarantee that their students will all have the same basic knowledge? How will we accurately measure their relative worth?  

> Salviati: They can’t, and we won’t. Just like in real life. Ultimately you have to face the fact that people are all different, and that’s just fine. In any case, there’s no urgency. So a person graduates from high school not knowing the half-angle formulas (as if they do now!) So what? 

Right after I finished reading this moving lament I discovered [`3blue1brown`][3blue1brown] Youtube channel. I watched his Linear Algebra series and in two minutes I could understand more of matrices than what I could after many hours plowing through a textbook. And thanks to his amazing visualizations I could also educate my sensibility towards that elusive mathematical beauty Lockhart speaks about in his article. 

Sanderson (they guy behind 3blue1brown) preludes his sixth video on linear algebra with the following quote:
> The purpose of computation is insight, not numbers. -Richard Hamming.

And in the following video he says:
> I'm not going to talk about the method for computing these things (inverse matrices, column space, rank, null space), and some would argue that that's pretty important. (...) I think most of the value that I actually have to add here is on the intuition half. Plus, we usually get software to compute this stuff for us anyway.

So if we combine Lockhart and Sanderson we get from them these two halves. On the one side there's computation (the applying of formulas/mechanical rote procedures to get results that will get us passing grades), and on the other side: the intuition, the insight, the beauty, the art, the joy of the hunt.

"Dude, I thought this post was about programming..." Look, many programmers, like myself, are a bit like [`Cate Blanchett's character on Indiana Jones 4`][I want to know] (yes, I actually love this film). We want to know and we want to know, 'everything'. Whatever 'everything' means. 

At this point I have to wear my psychotherapist hat and say a few things. And sorry if you don't see a clear connection between the initial Math rant and what follows. I think that to 'understand something' is not a very human impulse. I sense shame and anger behind such a convoluted purpose. 

Robert Oppenheimer says [`the following`][sweet] about what drives scientists:
> "(...) it is in my judgment in these things that when you see something that is technically sweet you go ahead and do it and you argue about what to do about it only after you have had your technical success. That is the way it was with the atomic bomb."

Something sweet. One could say in the 21st century: something cool (or whatever new word young people use nowadays to convey the same meaning). He goes on about the fascination of how stuff works. Notice I see a difference between 'how something works' and 'wanting to understand' something. To wonder about what makes something move is not akin to understanding something. 

A desire to understand is a desire to be in control of the stuff you want to understand. Is a desire of keeping it in check. To have the upper hand over it. In a way, one feels humiliated by the thing. Understanding it, is a revenge. There's no love towards the thing, and there cannot be with such obscure motivations. You're jumping over it with pins and needles trying to stop it from being so annoyingly complex.

In programming, we usually want to understand something when we have no idea how to begin to tackle a certain problem. So we think that going through 'the fundamentals' will be a good first step. But usually it isn't. Cache mechanisms, thorny concurrency issues, quirks of deep thick layered ORMs, mysteriously high DB CPU usage... insert here your own confusing mess you had to address last week. One cannot be blamed for trying but there's a point in which you have to learn to love the problem.

Not the abstract problem of 'concurrency', 'DB CPU usage', 'Hibernate 6 vs 5'. You have to learn to carve something from the chaos and love the highly specific problem in front of you. If you are lucky then whatever you need is not in Google and ChatGPT won't help you that much. At this point you are like Pythagoras attempting to measure the diagonal of a square and about to discover irrational numbers. And you need irrational numbers to solve your issue. But you don't give a damn about irrational numbers, you just want to figure out that diagonal. 

The dreaded imposter syndrome will punish you afterwards: "You don't even know what you just did to fix the issue. Shame. Shame. Shame." 

Maybe, sort of, in a way, but not completely, right? In a way is true because the square remains invisible to you. You did your diagonal, fixed the issue and moved on. You can lie to yourself and your colleagues and go on describing the square you weren't even able to see. And maybe you will never see it (and you can rest assured many of those that say 'they totally see a square' won't do either). But eventually you will see something. The glorious outline of a square will emerge as the background of all those hard earned crisscrossed diagonals. 

Or maybe not. 

Maybe, like some of those AI bros say, we are all nothing but a bunch of [`stochastic parrots`][parrots]. Could be. I think there's only one way to find out. 

[3blue1brown]: https://www.youtube.com/@3blue1brown
[I want to know]: https://www.youtube.com/watch?v=ohnkD-gjNVQ
[sweet]: https://ask.metafilter.com/263561/What-did-Robert-Oppenheimer-say-about-scientists-drive-to-get-results
[parrots]: https://en.wikipedia.org/wiki/Stochastic_parrot