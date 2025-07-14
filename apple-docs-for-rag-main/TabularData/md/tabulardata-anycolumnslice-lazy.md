

- TabularData
- AnyColumnSlice
-  lazy 

Instance Property

# lazy

A sequence containing the same elements as this sequence, but on which some operations, such as `map` and `filter`, are implemented lazily.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var lazy: LazySequence { get }
```

## See Also

### Creating a Derivative Column Slice

func reversed() -> ReversedCollection&lt;Self>

Returns a view presenting the elements of the collection in reverse order.

