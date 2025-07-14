

- Swift
- Set
-  init() 

Initializer

# init()

Creates an empty set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

Available when `Element` conforms to `Hashable`.

## Discussion

This is equivalent to initializing with an empty array literal. For example:

```
var emptySet = Set()
print(emptySet.isEmpty)
// Prints "true"

emptySet = []
print(emptySet.isEmpty)
// Prints "true"
```

## See Also

### Creating a Set

init(minimumCapacity: Int)

Creates an empty set with preallocated space for at least the specified number of elements.

init&lt;S>(S)

Creates a new set from a finite sequence of items.

init&lt;Source>(Source)

Creates a new set from a finite sequence of items.

