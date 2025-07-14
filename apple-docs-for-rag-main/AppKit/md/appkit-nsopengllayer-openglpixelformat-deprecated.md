

- AppKit
- NSOpenGLLayer
-  openGLPixelFormat Deprecated

Instance Property

# openGLPixelFormat

Provides access to the layer’s associated OpenGL pixel format.

macOS 10.6–10.14Deprecated

``` source
var openGLPixelFormat: NSOpenGLPixelFormat? { get set }
```

Deprecated

Please use CAMetalLayer instead.

## Discussion

Subclasses shouldn’t invoke `setOpenGLPixelFormat:`, but can override it if desired to intercept assignment of the layer’s pixel format.

## See Also

### Managing the Pixel Format

func openGLPixelFormat(forDisplayMask: UInt32) -> NSOpenGLPixelFormat

Returns the OpenGL pixel format suitable for the specified displays.

Deprecated

