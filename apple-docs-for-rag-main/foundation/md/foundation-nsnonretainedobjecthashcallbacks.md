

- Foundation
-  NSNonRetainedObjectHashCallBacks 

Global Variable

# NSNonRetainedObjectHashCallBacks

For sets of objects, but without retaining/releasing.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSNonRetainedObjectHashCallBacks: NSHashTableCallBacks
```

## See Also

### Constants

let NSIntegerHashCallBacks: NSHashTableCallBacks

For sets of `NSInteger`-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

let NSNonOwnedPointerHashCallBacks: NSHashTableCallBacks

For sets of pointers, hashed by address.

let NSObjectHashCallBacks: NSHashTableCallBacks

For sets of objects (similar to `NSSet`).

let NSOwnedObjectIdentityHashCallBacks: NSHashTableCallBacks

For sets of objects, with transfer of ownership upon insertion, using pointer equality.

let NSOwnedPointerHashCallBacks: NSHashTableCallBacks

For sets of pointers, with transfer of ownership upon insertion.

let NSPointerToStructHashCallBacks: NSHashTableCallBacks

For sets of pointers to structs, when the first field of the struct is `int`-sized.

