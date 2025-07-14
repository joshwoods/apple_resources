

- AppKit
- NSOpenGLContext
-  cglContextObj Deprecated

Instance Property

# cglContextObj

Returns the low-level, platform-specific Core OpenGL (CGL) context object represented by the receiver.

macOS 10.0–10.14Deprecated

``` source
var cglContextObj: CGLContextObj? { get }
```

Deprecated

Please use Metal or MetalKit.

## Return Value

A pointer to the CGLContextObj data type represented by the receiver.

