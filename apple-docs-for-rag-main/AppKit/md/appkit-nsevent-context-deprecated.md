

- AppKit
- NSEvent
-  context Deprecated

Instance Property

# context

The display graphics context for this event.

macOS 10.0–10.12Deprecated

``` source
var context: NSGraphicsContext? { get }
```

Deprecated

This method always returns `nil`. If you need access to the current drawing context, use current inside of a draw operation.

