

- AppKit
- NSOpenGLContext
-  clearCurrentContext() Deprecated

Type Method

# clearCurrentContext()

Clears the current context.

macOS 10.0–10.14Deprecated

``` source
class func clearCurrentContext()
```

Deprecated

Please use Metal or MetalKit.

## Discussion

Until you issue a subsequent call to the makeCurrentContext() method, OpenGL calls do nothing.

## See Also

### Managing the Current Context

class var current: NSOpenGLContext?

Returns the current OpenGL graphics context.

Deprecated

func makeCurrentContext()

Sets the context as the current OpenGL context object.

Deprecated

