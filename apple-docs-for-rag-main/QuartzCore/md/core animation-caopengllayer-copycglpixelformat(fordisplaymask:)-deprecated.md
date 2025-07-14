

- Core Animation
- CAOpenGLLayer
-  copyCGLPixelFormat(forDisplayMask:) Deprecated

Instance Method

# copyCGLPixelFormat(forDisplayMask:)

Returns the OpenGL pixel format suitable for rendering to the set of displays specified by the display mask.

Mac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.14Deprecated

``` source
func copyCGLPixelFormat(forDisplayMask mask: UInt32) -> CGLPixelFormatObj
```

Deprecated

OpenGL is deprecated

## Parameters 

`mask`  

The display mask the OpenGL content will be rendered on.

## Discussion

This method is called when a pixel format object is needed for the receiver. The default implementation returns a 32bpp fixed point pixelf format, with the `NoRecovery` and `Accelerated` flags set.

You should not call this method directly, it is intended to be overridden by subclasses.

## See Also

### Managing Pixel Format

func releaseCGLPixelFormat(CGLPixelFormatObj)

Releases the specified OpenGL pixel format object.

Deprecated

