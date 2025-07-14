

- Foundation
-  NSNonOwnedPointerMapKeyCallBacks 

Global Variable

# NSNonOwnedPointerMapKeyCallBacks

For keys that are pointers not freed.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
let NSNonOwnedPointerMapKeyCallBacks: NSMapTableKeyCallBacks
```

## See Also

### Constants

let NSIntegerMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointer-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

let NSIntMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointer-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

Deprecated

let NSNonOwnedPointerOrNullMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointers not freed, or `NULL`.

let NSNonRetainedObjectMapKeyCallBacks: NSMapTableKeyCallBacks

For sets of objects, but without retaining/releasing.

let NSObjectMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are objects.

let NSOwnedPointerMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointers, with transfer of ownership upon insertion.

