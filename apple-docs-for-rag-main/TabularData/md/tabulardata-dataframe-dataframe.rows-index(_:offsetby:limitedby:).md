

- TabularData
- DataFrame
- DataFrame.Rows
-  index(\_:offsetBy:limitedBy:) 

Instance Method

# index(\_:offsetBy:limitedBy:)

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func index(
    _ i: Self.Index,
    offsetBy distance: Int,
    limitedBy limit: Self.Index
) -> Self.Index?
```

## See Also

### Retrieving an Index

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

func firstIndex(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func index(Self.Index, offsetBy: Int) -> Self.Index

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func formIndex(inout Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Bool

Offsets the given index by the specified distance, or so that it equals the given limiting index.

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

