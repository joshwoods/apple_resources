

- Swift
- String
-  underestimatedCount 

Instance Property

# underestimatedCount

A value less than or equal to the number of elements in the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var underestimatedCount: Int { get }
```

## Discussion

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

## See Also

### Iterating over a String’s Characters

func forEach((Self.Element) throws -> Void) rethrows

Calls the given closure on each element in the sequence in the same order as a `for`-`in` loop.

func enumerated() -> EnumeratedSequence&lt;Self>

Returns a sequence of pairs (*n*, *x*), where *n* represents a consecutive integer starting at zero and *x* represents an element of the sequence.

func makeIterator() -> String.Iterator

Returns an iterator over the elements of the collection.

