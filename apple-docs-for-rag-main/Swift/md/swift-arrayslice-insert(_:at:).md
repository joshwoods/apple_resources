

- Swift
- ArraySlice
-  insert(\_:at:) 

Instance Method

# insert(\_:at:)

Inserts a new element at the specified position.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func insert(
    _ newElement: Element,
    at i: Int
)
```

## Parameters 

`newElement`  

The new element to insert into the array.

`i`  

The position at which to insert the new element. `index` must be a valid index of the array or equal to its `endIndex` property.

## Discussion

The new element is inserted before the element currently at the specified index. If you pass the array’s `endIndex` property as the `index` parameter, the new element is appended to the array.

```
var numbers = [1, 2, 3, 4, 5]
numbers.insert(100, at: 3)
numbers.insert(200, at: numbers.endIndex)

print(numbers)
// Prints "[1, 2, 3, 100, 4, 5, 200]"
```

Complexity

O(*n*), where *n* is the length of the array. If `i == endIndex`, this method is equivalent to `append(_:)`.

