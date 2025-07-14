

- Swift
- ContiguousArray
-  suffix(\_:) 

Instance Method

# suffix(\_:)

Returns a subsequence, up to the given maximum length, containing the final elements of the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func suffix(_ maxLength: Int) -> Self.SubSequence
```

## Parameters 

`maxLength`  

The maximum number of elements to return. `maxLength` must be greater than or equal to zero.

## Return Value

A subsequence terminating at the end of the collection with at most `maxLength` elements.

## Discussion

If the maximum length exceeds the number of elements in the collection, the result contains the entire collection.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.suffix(2))
// Prints "[4, 5]"
print(numbers.suffix(10))
// Prints "[1, 2, 3, 4, 5]"
```

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*k*), where *k* is equal to `maxLength`.

