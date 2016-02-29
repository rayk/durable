# Durable

Zero overhead library that provides durable persistence to object with least about
of overhead as possible. The intended use case of durable is to provide permanence
to object close to where they are used and required. In manner that does not assume
the underlying medium or overall data housing strategy.

There are only to main themes in this library, firstly that 'storing' objects is
not a seperate funciton external to the object or data structure, at least from
the perspective of a programer using durable.

The act of declaring of a data structure, class or a particular object instance
as durable is all that is required.

Accessing a durable object or data structure just entails having a reference
to it like any other object in memory.

Unpinning all of this is that only immutable persistence datastructure and objects
are acceptable to durable. That all post construction interactions with the
object or datastructure that is durable is async via a future of stream.
