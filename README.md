# Research Papers on Programming Languages

## On Linear Types, Ownerships and Alias Control

- [Capabilities for Uniqueness and Borrowing (ECOOP 2010)]
(http://lampwww.epfl.ch/~phaller/doc/haller-odersky10-Capabilities_for_uniqueness_and_borrowing.pdf): 
Haller and Odersky designed and implemented a type system which uses
capabilities to model uniqueness and borrowing. It offers "external uniqueness",
which is a more strict uniqueness in which the only access path to all
references inside an unique object is through the object itself. In other words,
no "shared" references are allowed inside an unique object. Atomic operations
are offered for transfering unique values and merging unique values.

- [A Type System for Borrowing Permissions (POPL 2012)](https://www.cs.cmu.edu/~kbierhof/papers/borrowing-permissions.pdf):
This type system covers different types of permissions such as unique,
none, immutable, local immutable, etc. A particular kind of permission called "local
permission" is supported by this system, which is useful for permission splitting and
combining. The system also supports "changing permissions", which is part of a method's
contract, and is similar to the input and output permissions specified for a method type
in Fractional Permissions.

- [Modular Typestate Checking of Aliased Objects (OOPSLA 2007)](https://www.cs.cmu.edu/~kbierhof/papers/typestate-verification.pdf):
a modular typestate checking tool based on a concept called _access
permissions_, which is high-level abstraction of Fractional Permissions and is
used to capture different patterns of them.
