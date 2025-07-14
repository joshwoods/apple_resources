

- Core Animation
- CAOpenGLLayer
-  releaseCGLContext(\_:) Deprecated

Instance Method

# releaseCGLContext(\_:)

Releases the specified rendering context.

Mac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.14Deprecated

``` source
func releaseCGLContext(_ ctx: CGLContextObj)
```

Deprecated

OpenGL is deprecated

## Parameters 

`ctx`  

The rendering context to release.

## Discussion

This method is called when the OpenGL context that was previously returned by copyCGLContext(forPixelFormat:) is no longer needed.

You should not call this method directly, it is intended to be overridden by subclasses.

## See Also

### Managing the Rendering Context

func copyCGLContext(forPixelFormat: CGLPixelFormatObj) -> CGLContextObj

Returns the rendering context the receiver requires for the specified pixel format.

Deprecated

