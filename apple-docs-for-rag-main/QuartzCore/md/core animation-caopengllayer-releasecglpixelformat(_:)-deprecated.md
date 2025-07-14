

- Core Animation
- CAOpenGLLayer
-  releaseCGLPixelFormat(\_:) Deprecated

Instance Method

# releaseCGLPixelFormat(\_:)

Releases the specified OpenGL pixel format object.

Mac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.14Deprecated

``` source
func releaseCGLPixelFormat(_ pf: CGLPixelFormatObj)
```

Deprecated

OpenGL is deprecated

## Parameters 

`pf`  

The pixel format object to release.

## Discussion

This method is called when the OpenGL pixel format that was previously returned by copyCGLContext(forPixelFormat:).

You should not call this method directly, it is intended to be overridden by subclasses.

## See Also

### Managing Pixel Format

func copyCGLPixelFormat(forDisplayMask: UInt32) -> CGLPixelFormatObj

Returns the OpenGL pixel format suitable for rendering to the set of displays specified by the display mask.

Deprecated

