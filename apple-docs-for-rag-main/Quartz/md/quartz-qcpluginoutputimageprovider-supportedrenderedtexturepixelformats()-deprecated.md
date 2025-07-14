

- Quartz
- QCPlugInOutputImageProvider
-  supportedRenderedTexturePixelFormats() Deprecated

Instance Method

# supportedRenderedTexturePixelFormats()

Returns a list of pixel formats that are supported for rendering to an onscreen OpenGL context.

macOS 10.5–10.14Deprecated

``` source
optional func supportedRenderedTexturePixelFormats() -> [Any]!
```

Deprecated

Quartz Composer OpenGL API deprecated. (Define QC_SILENCE_GL_DEPRECATION to silence these warnings)

## Return Value

Returns the list of texture pixel formats supported by copyRenderedTexture(forCGLContext:pixelFormat:bounds:isFlipped:) or `nil` if not supported.

## Discussion

If this method returns nil, then Quartz Composer calls canRender(withCGLContext:) /render(withCGLContext:forBounds:).

## See Also

### Providing Information About the Rendering Destination

func supportedBufferPixelFormats() -> [Any]!

Returns a list of pixel formats that are supported for rendering to a memory buffer.

Deprecated

func canRender(withCGLContext: CGLContextObj!) -> Bool

Returns whether the image data can be rendered into the provided CGL context.

Deprecated

