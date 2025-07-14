

- Swift
- Dictionary
-  lazy 

Instance Property

# lazy

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var lazy: LazySequence { get }
```

## See Also

### Iterating over Keys and Values

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func makeIterator() -> Dictionary&lt;Key, Value>.Iterator

Returns an iterator over the dictionary’s key-value pairs.

var underestimatedCount: Int

A value less than or equal to the number of elements in the collection.

