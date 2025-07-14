

- AppKit
- NSOpenGLPixelFormat
-  cglPixelFormatObj Deprecated

Instance Property

# cglPixelFormatObj

The low-level, platform-specific Core OpenGL (CGL) pixel format object represented by the receiver.

macOS 10.0–10.14Deprecated

``` source
var cglPixelFormatObj: CGLPixelFormatObj? { get }
```

Deprecated

Please use Metal or MetalKit.

## Return Value

A pointer to the underlying `CGLPixelFormatObj` object.

## See Also

### Managing the Pixel Format

func getValues(UnsafeMutablePointer&lt;GLint>, forAttribute: NSOpenGLPixelFormatAttribute, forVirtualScreen: GLint)

Gets the value for the specified pixel format attribute.

Deprecated

var numberOfVirtualScreens: GLint

The number of virtual screens associated with the OpenGL pixel format.

Deprecated

