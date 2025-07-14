

- AppKit
- NSOpenGLView
-  openGLContext Deprecated

Instance Property

# openGLContext

The NSOpenGLContext object associated with the receiver.

macOS 10.0–10.14Deprecated

``` source
@MainActor
var openGLContext: NSOpenGLContext? { get set }
```

Deprecated

Please use MTKView instead.

## Discussion

If the receiver has no associated context object, a new `NSOpenGLContext` object is created. The new object is initialized with the receiver’s pixel format information.

## See Also

### Related Documentation

var pixelFormat: NSOpenGLPixelFormat?

The NSOpenGLPixelFormat object associated with the receiver.

Deprecated

### Managing the NSOpenGLContext

func prepareOpenGL()

Used by subclasses to initialize OpenGL state.

Deprecated

func clearGLContext()

Releases the NSOpenGLContext object associated with the view.

Deprecated

