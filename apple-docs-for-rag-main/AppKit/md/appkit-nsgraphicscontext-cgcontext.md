

- AppKit
- NSGraphicsContext
-  cgContext 

Instance Property

# cgContext

The Core Graphics context, which is a low-level, platform-specific graphics context.

macOS 10.10+

``` source
var cgContext: CGContext { get }
```

## See Also

### Managing the Current Context

class var current: NSGraphicsContext?

Returns the current graphics context of the current thread.

var graphicsPort: UnsafeMutableRawPointer

The low-level, platform-specific graphics context represented by the graphic port.

Deprecated

