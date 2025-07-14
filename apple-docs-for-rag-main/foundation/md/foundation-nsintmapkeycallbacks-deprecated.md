

- Foundation
-  NSIntMapKeyCallBacks Deprecated

Global Variable

# NSIntMapKeyCallBacks

For keys that are pointer-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

tvOS 9.0–9.0DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
let NSIntMapKeyCallBacks: NSMapTableKeyCallBacks
```

Deprecated

Use `NSIntegerMapKeyCallBacks` instead.

## See Also

### Constants

let NSIntegerMapKeyCallBacks: NSMapTableKeyCallBacks

For keys that are pointer-sized quantities or smaller (for example, `int`, `long`, or `unichar`).

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

