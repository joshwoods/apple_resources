

- AppKit
- NSOpenGLView
-  clearGLContext() Deprecated

Instance Method

# clearGLContext()

Releases the NSOpenGLContext object associated with the view.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func clearGLContext()
```

Deprecated

Please use MTKView instead.

## Discussion

If necessary, this method calls the clearDrawable() method of the context object before releasing it.

## See Also

### Managing the NSOpenGLContext

func prepareOpenGL()

Used by subclasses to initialize OpenGL state.

Deprecated

var openGLContext: NSOpenGLContext?

The NSOpenGLContext object associated with the receiver.

Deprecated

