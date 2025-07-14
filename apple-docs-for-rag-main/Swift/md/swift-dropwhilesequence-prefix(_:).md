

- Swift
- DropWhileSequence
-  prefix(\_:) 

Instance Method

# prefix(\_:)

Returns a sequence, up to the specified maximum length, containing the initial elements of the sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func prefix(_ maxLength: Int) -> PrefixSequence
```

## Parameters 

`maxLength`  

The maximum number of elements to return. The value of `maxLength` must be greater than or equal to zero.

## Return Value

A sequence starting at the beginning of this sequence with at most `maxLength` elements.

## Discussion

If the maximum length exceeds the number of elements in the sequence, the result contains all the elements in the sequence.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.prefix(2))
// Prints "[1, 2]"
print(numbers.prefix(10))
// Prints "[1, 2, 3, 4, 5]"
```

Complexity

O(1)

