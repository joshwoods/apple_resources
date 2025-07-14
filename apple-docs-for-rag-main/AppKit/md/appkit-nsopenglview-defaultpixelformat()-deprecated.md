

- AppKit
- NSOpenGLView
-  defaultPixelFormat() Deprecated

Type Method

# defaultPixelFormat()

Returns a default NSOpenGLPixelFormat object.

macOS 10.0–10.14Deprecated

``` source
@MainActor
class func defaultPixelFormat() -> NSOpenGLPixelFormat
```

Deprecated

Please use MTKView instead.

## Return Value

A pixel format object with no attributes set.

## Discussion

Typically used with the initializer init(frame:pixelFormat:), this object has no attributes set.

## See Also

### Managing the NSOpenGLPixelFormat

var pixelFormat: NSOpenGLPixelFormat?

The NSOpenGLPixelFormat object associated with the receiver.

Deprecated

