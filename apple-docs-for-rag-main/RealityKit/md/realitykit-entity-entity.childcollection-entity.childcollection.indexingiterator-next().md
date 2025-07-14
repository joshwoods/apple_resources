

- RealityKit
- Entity
- Entity.ChildCollection
- Entity.ChildCollection.IndexingIterator
-  next() 

Instance Method

# next()

Advances to the next element and returns it, or `nil` if no next element exists.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
mutating func next() -> Elements.Element?
```

Available when `Elements` conforms to `Collection`.

## Return Value

The next element in the underlying sequence, if a next element exists; otherwise, `nil`.

## Discussion

Repeatedly calling this method returns, in order, all the elements of the underlying sequence. As soon as the sequence has run out of elements, all subsequent calls return `nil`.

You must not call this method if any other copy of this iterator has been advanced with a call to its `next()` method.

The following example shows how an iterator can be used explicitly to emulate a `for`-`in` loop. First, retrieve a sequence’s iterator, and then call the iterator’s `next()` method until it returns `nil`.

```
let numbers = [2, 3, 5, 7]
var numbersIterator = numbers.makeIterator()

while let num = numbersIterator.next() {
    print(num)
}
// Prints "2"
// Prints "3"
// Prints "5"
// Prints "7"
```

## See Also

### Iterating over the collection

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func makeIterator() -> Self

Returns an iterator over the elements of this sequence.

typealias Iterator

A type that provides the sequence’s iteration interface and encapsulates its iteration state.

typealias Element

The type of element traversed by the iterator.

var underestimatedCount: Int

A value less than or equal to the number of elements in the sequence, calculated nondestructively.

