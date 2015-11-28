# Research Papers on Programming Languages

A collection of papers that I've read or plan to read.

## On Linear Types, Ownerships, and Alias Control

- [Promises: Limited Specifications for Analysis and Manipulations (ICSE 98)](http://www.cs.uwm.edu/faculty/boyland/papers/promises.html)

- [Data groups: specifying the modification of extended state (OOPSLA 98)](http://research.microsoft.com/en-us/um/people/leino/papers/krml83.pdf)

- [An Object-Oriented Effects System (ECOOP 1999)](http://www.lirmm.fr/~ducour/Doc-objets/ECOOP/papers/1628/16280205.pdf)

- [Modular Typestate Checking of Aliased Objects (OOPSLA 07)](https://www.cs.cmu.edu/~kbierhof/papers/typestate-verification.pdf):
a modular typestate checking tool based on a concept called _access
permissions_, which is high-level abstraction of Fractional Permissions and is
used to capture different patterns of them.

- [Capabilities for Uniqueness and Borrowing (ECOOP 10)](http://lampwww.epfl.ch/~phaller/doc/haller-odersky10-Capabilities_for_uniqueness_and_borrowing.pdf): 
Haller and Odersky designed and implemented a type system which uses
capabilities to model uniqueness and borrowing. It offers "external uniqueness",
which is a more strict uniqueness in which the only access path to all
references inside an unique object is through the object itself. In other words,
no "shared" references are allowed inside an unique object. Atomic operations
are offered for transfering unique values and merging unique values.

- [A Type System for Borrowing Permissions (POPL 12)](https://www.cs.cmu.edu/~kbierhof/papers/borrowing-permissions.pdf):
This type system covers different types of permissions such as unique,
none, immutable, local immutable, etc. A particular kind of permission called "local
permission" is supported by this system, which is useful for permission splitting and
combining. The system also supports "changing permissions", which is part of a method's
contract, and is similar to the input and output permissions specified for a method type
in Fractional Permissions.

## Gradual Typing

- [Soft Typing (PLDI 1991)](http://citeseerx.ist.psu.edu/viewdoc/download?doi=10.1.1.24.9333&rep=rep1&type=pdf)

- [Gradual Typing for Functional Languages (SFP 06)](https://www.cs.colorado.edu/~siek/pubs/pubs/2006/siek06:_gradual.pdf)

- [Gradual Typing for Objects (ECOOP 07)](http://ecee.colorado.edu/~siek/gradual-obj.pdf):
combining static and dynamic typing for OO languages. Type annotation is optional, and in case
it is missing, a `?` type is used. During type checking, type equality is replaced
with _type consistency_, which can also be combined with subtyping. A gradual type system,
(which is based on the object calculus from Abadi and Cardelli) and its semantics are given in the paper.
The system is proven sound using machine-checked proofs.


