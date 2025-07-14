

- Foundation
-  NSIntegerMapKeyCallBacks 

Global Variable

# NSIntegerMapKeyCallBacks

For keys that are pointer-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

macOS 10.5+

``` source
let NSIntegerMapKeyCallBacks: NSMapTableKeyCallBacks
```

## See Also

### Constants

let NSIntMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointer-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

Deprecated

let NSNonOwnedPointerMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointers not freed.

let NSNonOwnedPointerOrNullMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointers not freed, or `NULL`.

let NSNonRetainedObjectMapKeyCallBacks: NSMapTableKeyCallBacks

For sets of objects, but without retaining/releasing.

let NSObjectMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are objects.

let NSOwnedPointerMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointers, with transfer of ownership upon insertion.

