

- AppKit
- NSOpenGLView
-  prepareOpenGL() Deprecated

Instance Method

# prepareOpenGL()

Used by subclasses to initialize OpenGL state.

macOS 10.0–10.14Deprecated

``` source
@MainActor
func prepareOpenGL()
```

Deprecated

Please use MTKView instead.

## Discussion

This method is called only once after the OpenGL context is made the current context. Subclasses that implement this method can use it to configure the Open GL state in preparation for drawing.

## See Also

### Managing the NSOpenGLContext

func clearGLContext()

Releases the NSOpenGLContext object associated with the view.

Deprecated

var openGLContext: NSOpenGLContext?

The NSOpenGLContext object associated with the receiver.

Deprecated

