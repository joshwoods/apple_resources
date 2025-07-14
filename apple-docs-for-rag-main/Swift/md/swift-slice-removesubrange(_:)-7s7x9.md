

- Swift
- Slice
-  removeSubrange(\_:) 

Instance Method

# removeSubrange(\_:)

Removes the specified subrange of elements from the collection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
mutating func removeSubrange(_ bounds: Range.Index>)
```

Available when `Base` conforms to `RangeReplaceableCollection`.

## Parameters 

`bounds`  

The subrange of the collection to remove. The bounds of the range must be valid indices of the collection.

## Discussion

```
var bugs = ["Aphid", "Bumblebee", "Cicada", "Damselfly", "Earwig"]
bugs.removeSubrange(1...3)
print(bugs)
// Prints "["Aphid", "Earwig"]"
```

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

