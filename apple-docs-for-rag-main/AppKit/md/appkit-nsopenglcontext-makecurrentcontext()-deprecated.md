

- AppKit
- NSOpenGLContext
-  makeCurrentContext() Deprecated

Instance Method

# makeCurrentContext()

Sets the context as the current OpenGL context object.

macOS 10.0–10.14Deprecated

``` source
func makeCurrentContext()
```

Deprecated

Please use Metal or MetalKit.

## Discussion

Subsequent OpenGL calls are rendered into the context defined by the receiver.

Note

A context is current on a per-thread basis. Multiple threads must serialize calls into the same context object.

## See Also

### Managing the Current Context

class func clearCurrentContext()

Clears the current context.

Deprecated

class var current: NSOpenGLContext?

Returns the current OpenGL graphics context.

Deprecated

