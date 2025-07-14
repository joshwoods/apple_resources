

- System
- FilePath
- FilePath.ComponentView
-  removeFirst(\_:) 

Instance Method

# removeFirst(\_:)

Removes the specified number of elements from the beginning of the collection.

SystemSwiftiOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
mutating func removeFirst(_ k: Int)
```

## Parameters 

`k`  

The number of elements to remove from the collection. `k` must be greater than or equal to zero and must not exceed the number of elements in the collection.

## Discussion

```
var bugs = ["Aphid", "Bumblebee", "Cicada", "Damselfly", "Earwig"]
bugs.removeFirst(3)
print(bugs)
// Prints "["Damselfly", "Earwig"]"
```

Calling this method may invalidate any existing indices for use with this collection.

Complexity

O(*n*), where *n* is the length of the collection.

