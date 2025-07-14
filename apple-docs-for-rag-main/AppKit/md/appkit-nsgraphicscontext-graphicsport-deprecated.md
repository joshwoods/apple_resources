

- AppKit
- NSGraphicsContext
-  graphicsPort Deprecated

Instance Property

# graphicsPort

The low-level, platform-specific graphics context represented by the graphic port.

macOS 10.0–10.14Deprecated

``` source
var graphicsPort: UnsafeMutableRawPointer { get }
```

Deprecated

Use cgContext instead.

## Discussion

In macOS, this is the Core Graphics context, a CGContext object (opaque type).

## See Also

### Managing the Current Context

class var current: NSGraphicsContext?

Returns the current graphics context of the current thread.

var cgContext: CGContext

The Core Graphics context, which is a low-level, platform-specific graphics context.

