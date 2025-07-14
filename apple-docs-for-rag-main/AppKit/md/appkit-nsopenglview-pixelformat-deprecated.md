

- AppKit
- NSOpenGLView
-  pixelFormat Deprecated

Instance Property

# pixelFormat

The NSOpenGLPixelFormat object associated with the receiver.

macOS 10.0–10.14Deprecated

``` source
@MainActor
var pixelFormat: NSOpenGLPixelFormat? { get set }
```

Deprecated

Please use MTKView instead.

## See Also

### Related Documentation

init?(frame: NSRect, pixelFormat: NSOpenGLPixelFormat?)

Returns an `NSOpenGLView` object initialized with the specified frame rectangle and pixel format.

Deprecated

### Managing the NSOpenGLPixelFormat

class func defaultPixelFormat() -> NSOpenGLPixelFormat

Returns a default NSOpenGLPixelFormat object.

Deprecated

