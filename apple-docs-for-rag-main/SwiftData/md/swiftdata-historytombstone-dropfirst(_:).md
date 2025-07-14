

- SwiftData
- HistoryTombstone
-  dropFirst(\_:) 

Instance Method

# dropFirst(\_:)

Returns a sequence containing all but the given number of initial elements.

SwiftDataSwiftiOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
func dropFirst(_ k: Int = 1) -> DropFirstSequence
```

## Parameters 

`k`  

The number of elements to drop from the beginning of the sequence. `k` must be greater than or equal to zero.

## Return Value

A sequence starting after the specified number of elements.

## Discussion

If the number of elements to drop exceeds the number of elements in the sequence, the result is an empty sequence.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.dropFirst(2))
// Prints "[3, 4, 5]"
print(numbers.dropFirst(10))
// Prints "[]"
```

Complexity

O(1), with O(*k*) deferred to each iteration of the result, where *k* is the number of elements to drop from the beginning of the sequence.

