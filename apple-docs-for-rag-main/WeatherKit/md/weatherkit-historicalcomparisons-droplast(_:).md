

- WeatherKit
- HistoricalComparisons
-  dropLast(\_:) 

Instance Method

# dropLast(\_:)

Returns a subsequence containing all but the specified number of final elements.

WeatherKitSwiftiOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
func dropLast(_ k: Int) -> Self.SubSequence
```

## Parameters 

`k`  

The number of elements to drop off the end of the collection. `k` must be greater than or equal to zero.

## Return Value

A subsequence that leaves off `k` elements from the end.

## Discussion

If the number of elements to drop exceeds the number of elements in the collection, the result is an empty subsequence.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.dropLast(2))
// Prints "[1, 2, 3]"
print(numbers.dropLast(10))
// Prints "[]"
```

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the number of elements to drop.

