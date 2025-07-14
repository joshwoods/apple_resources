

- Foundation
-  NSIntegerHashCallBacks 

Global Variable

# NSIntegerHashCallBacks

For sets of `NSInteger`-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

macOS 10.5+

``` source
let NSIntegerHashCallBacks: NSHashTableCallBacks
```

## See Also

### Constants

let NSNonOwnedPointerHashCallBacks: NSHashTableCallBacks

For sets of pointers, hashed by address.

let NSNonRetainedObjectHashCallBacks: NSHashTableCallBacks

For sets of objects, but without retaining/releasing.

let NSObjectHashCallBacks: NSHashTableCallBacks

For sets of objects (similar to `NSSet`).

let NSOwnedObjectIdentityHashCallBacks: NSHashTableCallBacks

For sets of objects, with transfer of ownership upon insertion, using pointer equality.

let NSOwnedPointerHashCallBacks: NSHashTableCallBacks

For sets of pointers, with transfer of ownership upon insertion.

let NSPointerToStructHashCallBacks: NSHashTableCallBacks

For sets of pointers to structs, when the first field of the struct is `int`-sized.

