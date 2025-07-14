

- AppKit
- NSOpenGLPixelFormat
-  numberOfVirtualScreens Deprecated

Instance Property

# numberOfVirtualScreens

The number of virtual screens associated with the OpenGL pixel format.

macOS 10.0–10.14Deprecated

``` source
var numberOfVirtualScreens: GLint { get }
```

Deprecated

Please use Metal or MetalKit.

## Return Value

The number of virtual screens.

## Discussion

When the attributes are set, OpenGL searches for drivers matching the requested attributes. Each matching driver drives a set of displays. For example, a graphics card in a portable computer might drive the internal screen and an external display. This portable computer would have one virtual screen. A desktop computer might have two different graphics cards, each driving one or more displays. The pairing of an OpenGL driver with its set of associated displays corresponds to one virtual screen. In the above examples, the portable computer would have one virtual screen, while the desktop computer would have two. Another desktop computer with a video card driving two displays at once would have one virtual screen.

For more information on virtual screens, consult OpenGL Programming Guide for Mac.

## See Also

### Managing the Pixel Format

var cglPixelFormatObj: CGLPixelFormatObj?

The low-level, platform-specific Core OpenGL (CGL) pixel format object represented by the receiver.

Deprecated

func getValues(UnsafeMutablePointer&lt;GLint>, forAttribute: NSOpenGLPixelFormatAttribute, forVirtualScreen: GLint)

Gets the value for the specified pixel format attribute.

Deprecated

