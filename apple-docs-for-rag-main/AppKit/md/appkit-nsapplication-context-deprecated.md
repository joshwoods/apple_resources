

- AppKit
- NSApplication
-  context Deprecated

Instance Property

# context

The graphics context associated with the app.

macOS 10.0–10.12Deprecated

``` source
@MainActor
var context: NSGraphicsContext? { get }
```

Deprecated

This method always returns nil. If you need access to the current drawing context, use \[NSGraphicsContext currentContext\] inside of a draw operation.

## Discussion

This property contains the graphics context most recently used by your app.

