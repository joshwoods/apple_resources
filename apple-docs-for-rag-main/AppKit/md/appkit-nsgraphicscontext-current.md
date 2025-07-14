

- AppKit
- NSGraphicsContext
-  current 

Type Property

# current

Returns the current graphics context of the current thread.

macOS

``` source
class var current: NSGraphicsContext? { get set }
```

## Return Value

The current graphics context of the current thread.

## Discussion

Returns an instance of a concrete subclass of NSGraphicsContext.

## See Also

### Managing the Current Context

var cgContext: CGContext

The Core Graphics context, which is a low-level, platform-specific graphics context.

var graphicsPort: UnsafeMutableRawPointer

The low-level, platform-specific graphics context represented by the graphic port.

Deprecated

