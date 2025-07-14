

- AppKit
- NSPathControl
-  menu 

Instance Property

# menu

The menu that is used for the path control’s cells.

macOS 10.5+

``` source
@MainActor
var menu: NSMenu? { get set }
```

## Discussion

This property overrides the NSView implementation of `menu` and forwards the message to the `NSPathControlCell`.

