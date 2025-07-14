

- Swift
- EnumeratedSequence
- EnumeratedSequence.Iterator
-  suffix(\_:) 

Instance Method

# suffix(\_:)

Returns a subsequence, up to the given maximum length, containing the final elements of the sequence.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func suffix(_ maxLength: Int) -> [Self.Element]
```

## Parameters 

`maxLength`  

The maximum number of elements to return. The value of `maxLength` must be greater than or equal to zero.

## Discussion

The sequence must be finite. If the maximum length exceeds the number of elements in the sequence, the result contains all the elements in the sequence.

```
let numbers = [1, 2, 3, 4, 5]
print(numbers.suffix(2))
// Prints "[4, 5]"
print(numbers.suffix(10))
// Prints "[1, 2, 3, 4, 5]"
```

Complexity

O(*n*), where *n* is the length of the sequence.

