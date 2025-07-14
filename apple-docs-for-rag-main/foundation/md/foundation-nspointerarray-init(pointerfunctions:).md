

- Foundation
- NSPointerArray
-  init(pointerFunctions:) 

Initializer

# init(pointerFunctions:)

Initializes the receiver to use the given functions.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(pointerFunctions functions: NSPointerFunctions)
```

## Parameters 

`functions`  

The pointer functions for the new instance.

## Return Value

The receiver, initialized to use the given functions.

## See Also

### Creating and Initializing a New Pointer Array

init(options: NSPointerFunctions.Options)

Initializes the receiver to use the given options.

class func strongObjects() -> NSPointerArray

Returns a new pointer array that maintains strong references to its elements.

class func weakObjects() -> NSPointerArray

Returns a new pointer array that maintains weak references to its elements.

