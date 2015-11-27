# Research Papers on Programming Languages

## On Linear Types

- [Capabilities for Uniqueness and Borrowing (ECOOP 2010)]
(http://lampwww.epfl.ch/~phaller/doc/haller-odersky10-Capabilities_for_uniqueness_and_borrowing.pdf): 
Haller and Odersky designed and implemented a type system which uses
capabilities to model uniqueness and borrowing. It offers "external uniqueness",
which is a more strict uniqueness in which the only access path to all
references inside an unique object is through the object itself. In other words,
no "shared" references are allowed inside an unique object. Atomic operations
are offered for transfering unique values and merging unique values.

- [A Type System for Borrowing Permissions (POPL 2012)](https://www.cs.cmu.edu/~kbierhof/papers/borrowing-permissions.pdf)
