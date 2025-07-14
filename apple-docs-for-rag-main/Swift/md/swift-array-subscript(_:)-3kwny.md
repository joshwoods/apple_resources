

- Swift
- Array
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
subscript(r: R) -> Self.SubSequence where R : RangeExpression, Self.Index == R.Bound { get set }
```

## See Also

### Accessing Elements

subscript(Int) -> Element

Accesses the element at the specified position.

var first: Self.Element?

The first element of the collection.

var last: Self.Element?

The last element of the collection.

subscript(Range&lt;Int>) -> ArraySlice&lt;Element>

Accesses a contiguous subrange of the array’s elements.

subscript&lt;R>(R) -> Self.SubSequence

Accesses the contiguous subrange of the collection’s elements specified by a range expression.

subscript((UnboundedRange_) -> ()) -> Self.SubSequence

func randomElement() -> Self.Element?

Returns a random element of the collection.

func randomElement&lt;T>(using: inout T) -> Self.Element?

Returns a random element of the collection, using the given generator as a source for randomness.

