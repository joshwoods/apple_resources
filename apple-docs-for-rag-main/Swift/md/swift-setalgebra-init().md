

- Swift
- SetAlgebra
-  init() 

Initializer

# init()

Creates an empty set.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

**Required** Default implementation provided.

## Discussion

This initializer is equivalent to initializing with an empty array literal. For example, you create an empty `Set` instance with either this initializer or with an empty array literal.

```
var emptySet = Set()
print(emptySet.isEmpty)
// Prints "true"

emptySet = []
print(emptySet.isEmpty)
// Prints "true"
```

## Default Implementations

### SetAlgebra Implementations

init()

Creates an empty option set.

