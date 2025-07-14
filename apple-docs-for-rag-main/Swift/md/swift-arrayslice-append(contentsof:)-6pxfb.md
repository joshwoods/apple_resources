

- Swift
- ArraySlice
-  append(contentsOf:) 

Instance Method

# append(contentsOf:)

Adds the elements of a sequence or collection to the end of this collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func append(contentsOf newElements: S) where S : Sequence, Self.Element == S.Element
```

## Parameters 

`newElements`  

The elements to append to the collection.

## Discussion

The collection being appended to allocates any additional necessary storage to hold the new elements.

The following example appends the elements of a `Range` instance to an array of integers:

```
var numbers = [1, 2, 3, 4, 5]
numbers.append(contentsOf: 10...15)
print(numbers)
// Prints "[1, 2, 3, 4, 5, 10, 11, 12, 13, 14, 15]"
```

Complexity

O(*m*), where *m* is the length of `newElements`.

