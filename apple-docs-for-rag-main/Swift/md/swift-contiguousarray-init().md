

- Swift
- ContiguousArray
-  init() 

Initializer

# init()

Creates a new, empty array.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.0+macOS 10.10+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init()
```

## Discussion

This is equivalent to initializing with an empty array literal. For example:

```
var emptyArray = Array()
print(emptyArray.isEmpty)
// Prints "true"

emptyArray = []
print(emptyArray.isEmpty)
// Prints "true"
```

