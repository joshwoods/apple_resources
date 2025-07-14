

- AppKit
- NSPrintOperation
-  current 

Type Property

# current

The current print operation for this thread.

macOS

``` source
@MainActor
class var current: NSPrintOperation? { get set }
```

## Return Value

The print operation object, or `nil` if there is no current operation.

