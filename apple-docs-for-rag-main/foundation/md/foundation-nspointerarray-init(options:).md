

- Foundation
- NSPointerArray
-  init(options:) 

Initializer

# init(options:)

Initializes the receiver to use the given options.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(options: NSPointerFunctions.Options = [])
```

## Parameters 

`options`  

The pointer functions options for the new instance.

## Return Value

The receiver, initialized to use the given options.

## See Also

### Related Documentation

Collections Programming Topics

### Creating and Initializing a New Pointer Array

init(pointerFunctions: NSPointerFunctions)

Initializes the receiver to use the given functions.

class func strongObjects() -> NSPointerArray

Returns a new pointer array that maintains strong references to its elements.

class func weakObjects() -> NSPointerArray

Returns a new pointer array that maintains weak references to its elements.

