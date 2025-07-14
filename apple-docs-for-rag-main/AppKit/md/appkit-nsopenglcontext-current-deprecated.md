

- AppKit
- NSOpenGLContext
-  current Deprecated

Type Property

# current

Returns the current OpenGL graphics context.

macOS 10.0–10.14Deprecated

``` source
class var current: NSOpenGLContext? { get }
```

Deprecated

Please use Metal or MetalKit.

## Return Value

The current OpenGL graphics context, or `nil` if no such object has been set.

## See Also

### Managing the Current Context

class func clearCurrentContext()

Clears the current context.

Deprecated

func makeCurrentContext()

Sets the context as the current OpenGL context object.

Deprecated

