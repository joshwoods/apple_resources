

- Foundation
- NSPointerArray
-  pointerFunctions 

Instance Property

# pointerFunctions

The functions in use by the receiver.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+macOS 10.5+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
@NSCopying
var pointerFunctions: NSPointerFunctions { get }
```

## Discussion

The returned object is a new `NSPointerFunctions` object that you can modify and/or use directly to create other pointer collections.

## See Also

### Getting the Pointer Functions

class NSPointerFunctions

An instance of `NSPointerFunctions` defines callout functions appropriate for managing a pointer reference held somewhere else.

