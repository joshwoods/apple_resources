

- Swift
- String
- String.UTF8View
-  dropFirst(\_:) 

Instance Method

# dropFirst(\_:)

Returns a subsequence containing all but the given number of initial elements.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func dropFirst(_ k: Int = 1) -> Self.SubSequence
```

## Parameters 

`k`  

The number of elements to drop from the beginning of the collection. `k` must be greater than or equal to zero.

## Return Value

A subsequence starting after the specified number of elements.

## Discussion

If the number of elements to drop exceeds the number of elements in the collection, the result is an empty subsequence.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.dropFirst(2))
// Prints "[3, 4, 5]"
print(numbers.dropFirst(10))
// Prints "[]"
```

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is the number of elements to drop from the beginning of the collection.

