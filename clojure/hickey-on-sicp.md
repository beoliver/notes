# SICP
### The Structure and Interpretation of Programming Languages.

It's not just data.

> As programmers, we should be alert to opportunities to identify the underlying abstractions in our programs and to build upon them and generalize them to create more powerful abstractions. This is not to say that one should always write programs in the most abstract way possible; expert programmers know how to choose the level of abstraction appropriate to their task. But it is important to be able to think in terms of these abstractions, so that we can be ready to apply them in new contexts. The significance of higher-order procedures is that they enable us to represent these abstractions explicitly as elements in our programming language, so that they can be handled just like other computational elements.

p102 SICP (Second Edition)


## Hickey on SICP

[Rich Hickey on clojure for SICP](https://groups.google.com/g/clojure/c/jyOuJFukpmE/m/aZjWHBnsQ74J?pli=1)

> Everyone's experience will be different, of course. Here's my 2 cents:

> I don't think SICP is a book about a programming language. It's a book about programming. It uses Scheme because Scheme is in many ways an atomic programming language. Lambda calculus + TCO for loops + Continuations for control abstraction + syntactic abstraction (macros) + mutable state for when you need it. It is very small. It is  sufficient.

> The book really deals with the issues in programming. Modularity, abstraction, state, data structures, concurrency etc. It provides descriptions and toy implementations of generic dispatch, objects, concurrency, lazy lists, (mutable) data structures, 'tagging' etc, designed to illuminate the issues.  

> Clojure is not an atomic programming language. I'm too tired/old/lazy to program with atoms. Clojure provides production implementations of generic dispatch, associative maps, metadata, concurrency infrastructure, persistent data structures, lazy seqs, polymorphic libraries etc etc. Much better implementations of some of the things you would be building by following along with SICP are in Clojure already.

> So the value in SICP would be in helping you understand programming concepts. If you already understand the concepts, Clojure lets you get on with writing interesting and robust programs much more quickly, IMO. And I don't think the core of Clojure is appreciably bigger than Scheme's. What do Schemers think?

> I think the Lisps prior to Clojure lead you towards a good path with functional programming and lists, only to leave you high and dry when it comes to the suite of data structures you need to write real programs, such data structures, when provided, being mutable and imperative. Prior Lisps were also designed before pervasive in-process concurrency, and before the value of high-performance polymorphic dispatch (e.g. virtual functions) as library infrastructure was well understood. Their libraries have decidedly limited polymorphism. Alas, there is no book on Clojure yet. But, to the extent Schemes go beyond the standard to provide more complete functionality (as most do), there are no books on that either. Just docs in both cases. Learning Scheme or Common Lisp on your way to Clojure is fine. There will be specifics that don't translate (from Scheme - no TCO, false/ nil/() differences, no continuations; from CL - Lisp-1, symbol/var dichotomy). But I personally don't think SICP will help you much with Clojure. YMMV.

> Rich

