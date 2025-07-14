

- AppKit
- NSOpenGLLayer
-  openGLContext(for:) Deprecated

Instance Method

# openGLContext(for:)

Returns the OpenGL context to use for the requested pixel format.

macOS 10.6–10.14Deprecated

``` source
func openGLContext(for pixelFormat: NSOpenGLPixelFormat) -> NSOpenGLContext
```

Deprecated

Please use CAMetalLayer instead.

## Parameters 

`pixelFormat`  

The pixel format.

## Return Value

An autoreleased NSOpenGLContext.

## See Also

### Managing the Rendering Context

var openGLContext: NSOpenGLContext?

The layer’s OpenGL context.

Deprecated

