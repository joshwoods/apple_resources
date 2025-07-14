

- System
- FilePath
- FilePath.ComponentView
-  append(\_:) 

Instance Method

# append(\_:)

Adds an element to the end of the collection.

SystemSwiftiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
mutating func append(_ newElement: Self.Element)
```

## Parameters 

`newElement`  

The element to append to the collection.

## Discussion

If the collection does not have sufficient capacity for another element, additional storage is allocated before appending `newElement`. The following example adds a new number to an array of integers:

```
var numbers = [1, 2, 3, 4, 5]
numbers.append(100)

print(numbers)
// Prints "[1, 2, 3, 4, 5, 100]"
```

Complexity

O(1) on average, over many calls to `append(_:)` on the same collection.

