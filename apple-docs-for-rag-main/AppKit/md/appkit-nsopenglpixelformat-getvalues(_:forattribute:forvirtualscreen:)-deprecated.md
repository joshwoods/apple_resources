

- AppKit
- NSOpenGLPixelFormat
-  getValues(\_:forAttribute:forVirtualScreen:) Deprecated

Instance Method

# getValues(\_:forAttribute:forVirtualScreen:)

Gets the value for the specified pixel format attribute.

macOS 10.0–10.14Deprecated

``` source
func getValues(
    _ vals: UnsafeMutablePointer,
    forAttribute attrib: NSOpenGLPixelFormatAttribute,
    forVirtualScreen screen: GLint
)
```

Deprecated

Please use Metal or MetalKit.

## Parameters 

`vals`  

On input, a pointer to a `long` variable. On output, the variable contains the value of the requested attribute.

`attrib`  

The requested attribute. For a list of attribute constants, see the table in Constants.

`screen`  

The screen from which you want to retrieve the attribute. This parameter must be a value between 0 and the number of virtual screens (numberOfVirtualScreens) minus 1.

## Discussion

Because the value for an attribute may be different on each virtual screen, the virtual screen must be specified along with the attribute.

## See Also

### Related Documentation

convenience init?(attributes: UnsafePointer&lt;NSOpenGLPixelFormatAttribute>)

Returns an OpenGL pixel format object initialized with specified pixel format attributes.

Deprecated

### Managing the Pixel Format

var cglPixelFormatObj: CGLPixelFormatObj?

The low-level, platform-specific Core OpenGL (CGL) pixel format object represented by the receiver.

Deprecated

var numberOfVirtualScreens: GLint

The number of virtual screens associated with the OpenGL pixel format.

Deprecated

