

- AppKit
- NSOpenGLLayer
-  openGLContext Deprecated

Instance Property

# openGLContext

The layer’s OpenGL context.

macOS 10.6–10.14Deprecated

``` source
var openGLContext: NSOpenGLContext? { get set }
```

Deprecated

Please use CAMetalLayer instead.

## Discussion

Provides access to the layer’s associated NSOpenGLContext. Subclasses shouldn’t invoke `setOpenGLContext:`, but can override it if desired to intercept assignment of the layer’s context.

## See Also

### Managing the Rendering Context

func openGLContext(for: NSOpenGLPixelFormat) -> NSOpenGLContext

Returns the OpenGL context to use for the requested pixel format.

Deprecated

