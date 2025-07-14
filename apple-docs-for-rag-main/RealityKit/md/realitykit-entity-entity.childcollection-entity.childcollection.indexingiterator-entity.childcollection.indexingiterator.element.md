

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
-  Entity.ChildCollection.IndexingIterator.Element 

Type Alias

# Entity.ChildCollection.IndexingIterator.Element

The type of element traversed by the iterator.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
typealias Element = Elements.Element
```

Available when `Elements` conforms to `Collection`.

## See Also

### Iterating over the collection

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func next() -> Elements.Element?

Advances to the next element and returns it, or `nil` if no next element exists.

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func makeIterator() -> Self

Returns an iterator over the elements of this sequence.

typealias Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

var underestimatedCount: Int

A value less than or equal to the number of elements in the sequence, calculated nondestructively.

