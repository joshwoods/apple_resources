

- Swift
- Set
-  makeIterator() 

Instance Method

# makeIterator()

Returns an iterator over the members of the set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func makeIterator() -> Set.Iterator
```

Available when `Element` conforms to `Hashable`.

## See Also

### Iterating over a Set

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

