

- TabularData
- FilledColumn
-  formIndex(\_:offsetBy:limitedBy:) 

Instance Method

# formIndex(\_:offsetBy:limitedBy:)

Offsets the given index by the specified distance, or so that it equals the given limiting index.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func formIndex(
    _ i: inout Self.Index,
    offsetBy distance: Int,
    limitedBy limit: Self.Index
) -> Bool
```

## Parameters 

`i`  

A valid index of the collection.

`distance`  

The distance to offset `i`. `distance` must not be negative unless the collection conforms to the `BidirectionalCollection` protocol.

`limit`  

A valid index of the collection to use as a limit. If `distance > 0`, a limit that is less than `i` has no effect. Likewise, if `distance 

## Return Value

`true` if `i` has been offset by exactly `distance` steps without going beyond `limit`; otherwise, `false`. When the return value is `false`, the value of `i` is equal to `limit`.

## Discussion

The value passed as `distance` must not offset `i` beyond the bounds of the collection, unless the index passed as `limit` prevents offsetting beyond those bounds.

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the absolute value of `distance`.

## See Also

### Retrieving an Index

var indices: DefaultIndices&lt;Self>

The indices that are valid for subscripting the collection, in ascending order.

func firstIndex(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

func firstIndex(where: (Self.Element) throws -> Bool) rethrows -> Self.Index?

Returns the first index in which an element of the collection satisfies the given predicate.

func index(Self.Index, offsetBy: Int) -> Self.Index

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

func formIndex(inout Self.Index, offsetBy: Int)

Offsets the given index by the specified distance.

func index(of: Self.Element) -> Self.Index?

Returns the first index where the specified value appears in the collection.

