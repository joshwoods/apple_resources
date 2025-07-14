

- AppKit
- NSOpenGLLayer
-  openGLPixelFormat(forDisplayMask:) Deprecated

Instance Method

# openGLPixelFormat(forDisplayMask:)

Returns the OpenGL pixel format suitable for the specified displays.

macOS 10.6–10.14Deprecated

``` source
func openGLPixelFormat(forDisplayMask mask: UInt32) -> NSOpenGLPixelFormat
```

Deprecated

Please use CAMetalLayer instead.

## Parameters 

`mask`  

A mask specifying the displays the returned NSOpenGLPixelFormat must be suitable for.

## Return Value

An autoreleased NSOpenGLPixelFormat object suitable for the displays.

## Discussion

You must include an NSOpenGLPFAScreenMask specification in the pixel format attribute list that’s used to instantiate the NSOpenGLPixelFormat.

## See Also

### Managing the Pixel Format

var openGLPixelFormat: NSOpenGLPixelFormat?

Provides access to the layer’s associated OpenGL pixel format.

Deprecated

