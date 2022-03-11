In this project, you will explore new techniques to represent algebraic data types (ADTs) more efficiently. You will work on the internals of a sophisticated, static compiler for the Virgil programming language and introduce new analysis and optimizations in this compiler.

A key data structure in functional languages and now appearing in many mainstream languages, algebraic data types (ADTs), also referred to as variants or sum types, are a feature that allows a programmer to define a fixed set of data forms that can be efficiently created, compared, and matched on. Typically immutable, such data structures can form trees and DAG structures and are suitable for a wide variety of use cases.

While these data structures are typically represented as garbage-collected objects (i.e. consume memory on the program heap), an exciting direction in compilers is to pack, unbox, and flatten such data structures so that they don't require allocating memory. When the compiler applies these optimizations, ADTs can rival even the best hand-tuned code in terms of performance and memory consumption.

This will be a very code-centric project. You will explore new algorithms and compiler transforms and implement them in an actual compiler. If your project is successful it will become part of the standard suite of optimizations for this language and likely lead to an ICFP publication.
