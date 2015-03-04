# POODR-notes
My notes on Sandi Metz's Practical OOD in Ruby book

#Intro
Design is important because all code is extremely likely to need modifications - because technology is changing, and because client needs are changing too. This is why OOD is so important, it makes modifying and extending code far easier - more cost-efficient, and also more pleasant to change. OOD implies seeing the world as objects that send each other messages.

#Chapter 1: Object-Oriented Design
OOD tries to manage dependencies, ensuring objects know as little as possible about each other, once again to facilitate change.

####Design tools are very useful, but must be used wisely.

SOLID - studies have proven the usefulness of these design principles.

Design Patterns are "simple and elegant solutions to specific problems in OO software design that make one's design more flexible, modular, reusable, and understandable". They can be a near-perfect open-source solution for the problem they solve, but must be applied to the right problems. 

A balance must be found between not using design tools, which leads to "I can add that feature but it will break everything"-type situations, to overdesign, where devs see patterns where none exist and apply principles inappropriately. Those will answer change requests with "no I can't add that feature, the app wasn't designed to do that".

####Why Agile is essential to good OOD 

Design should also go hand in hand with quick iterations (Agile) so the design can adjust regularly and evolve naturally. Big Upfront Design is against Agile principles, which say the product's design should be led by user feedback. BFUD can seem comforting to the client as he has a sense of what the product will look like and how long it will take to build it, but can be frustrating for the dev as he knows BFUD will never properly meet the user's needs. A client/dev blame game ends up happening; the dev if BFUD requirements are not built; the client if requirements don't meet user needs. The Agile Manifesto solves these tensions by saying certainty is impossible to have before building the application.

Because Agile implies constantly modifying your code, OOD is crucial.

####How to evaluate code quality and decide how qualitative your code should be

Programmers used to be evaluated on the number of lines of codes they produced, rewarding verbose devs and penalising efficient ones. Now there are Ruby gems to evaluate how well your code follows OOD principles. But they must be taken with a pinch of salt as they might read designs that over-anticipate the future, and be hard to change if the future is not as expected!

The ideal measurement would be cost per feature over the time interval that matters. It can be very short if you risk going out of business tomorrow; then best to build the feature in a rush and deal with technical debt later. You should also consider the amount of time you spend designing vs. the amount of time you'll get reaping the benefits of having designed well. The former obviously depends a lot on your skill level/experience.

####What makes OOD different

OO programming is different from procedural programming. In the latter, the user has to define the type of data it is using, and the operations it can run on it are pre-defined. Data and behaviour are completely separated. Ruby puts them together in an object. Objects invoke one another's behaviour by sending messages. Each objects contains the operations it can run, so Ruby doesn't need to know them, it just has to help the object send the operation to another. A class contains methods and attributes (definitions of variables). Ruby has some built-in classes that are of the class Class and correspond to the data types of procedural programming: String, Array, Fixnum, etc..

The focus of this chapter has been theory; it's now time for practice!

#Chapter 2: Designing Classes with a Single Responsibility

TBC!
