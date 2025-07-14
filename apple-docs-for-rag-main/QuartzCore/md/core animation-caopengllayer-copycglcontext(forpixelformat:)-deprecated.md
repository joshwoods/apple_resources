

- Core Animation
- CAOpenGLLayer
-  copyCGLContext(forPixelFormat:) Deprecated

Instance Method

# copyCGLContext(forPixelFormat:)

Returns the rendering context the receiver requires for the specified pixel format.

Mac Catalyst 13.1–13.1DeprecatedmacOS 10.5–10.14Deprecated

``` source
func copyCGLContext(forPixelFormat pf: CGLPixelFormatObj) -> CGLContextObj
```

Deprecated

OpenGL is deprecated

## Parameters 

`pf`  

The pixel format for the rendering context.

## Return Value

A new `CGLContext` with renderers for `pixelFormat`.

## Discussion

This method is called when a rendering context is needed by the receiver. The default implementation allocates a new context with a null share context.

You should not call this method directly, it is intended to be overridden by subclasses.

## See Also

### Managing the Rendering Context

func releaseCGLContext(CGLContextObj)

Releases the specified rendering context.

Deprecated

