

- AppKit
- NSOpenGLContext
-  currentVirtualScreen Deprecated

Instance Property

# currentVirtualScreen

Returns the current virtual screen for the OpenGL context.

macOS 10.0–10.14Deprecated

``` source
var currentVirtualScreen: GLint { get set }
```

Deprecated

Please use Metal or MetalKit.

## Return Value

The virtual screen number, which is a value between 0 and the number of virtual screens minus one.

