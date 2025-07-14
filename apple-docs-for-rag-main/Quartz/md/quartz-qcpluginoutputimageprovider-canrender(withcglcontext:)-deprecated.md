

- Quartz
- QCPlugInOutputImageProvider
-  canRender(withCGLContext:) Deprecated

Instance Method

# canRender(withCGLContext:)

Returns whether the image data can be rendered into the provided CGL context.

macOS 10.5–10.14Deprecated

``` source
optional func canRender(withCGLContext cgl_ctx: CGLContextObj!) -> Bool
```

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Parameters 

`cgl_ctx`  

The CGL context that your image will be rendered to.

## Return Value

true if the image can be rendered into this CGL context; otherwise false, in which case render(toBuffer:withBytesPerRow:pixelFormat:forBounds:) is called.

## Discussion

If your image can render using any OpenGL context, simply return true. If your code requires special extensions, you’ll need to check for them and then provide the appropriate return value. For more information on checking for OpenGL capabilities supported by the hardware, see OpenGL Programming Guide for Mac.

## See Also

### Providing Information About the Rendering Destination

func supportedBufferPixelFormats() -> [Any]!

Returns a list of pixel formats that are supported for rendering to a memory buffer.

Deprecated

func supportedRenderedTexturePixelFormats() -> [Any]!

Returns a list of pixel formats that are supported for rendering to an onscreen OpenGL context.

Deprecated

