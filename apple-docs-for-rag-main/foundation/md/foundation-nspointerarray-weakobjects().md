

- Foundation
- NSPointerArray
-  weakObjects() 

Type Method

# weakObjects()

Returns a new pointer array that maintains weak references to its elements.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.8+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
class func weakObjects() -> NSPointerArray
```

## Return Value

A new pointer array that maintains weak references to its elements.

## See Also

### Creating and Initializing a New Pointer Array

init(options: NSPointerFunctions.Options)

Initializes the receiver to use the given options.

init(pointerFunctions: NSPointerFunctions)

Initializes the receiver to use the given functions.

class func strongObjects() -> NSPointerArray

Returns a new pointer array that maintains strong references to its elements.

