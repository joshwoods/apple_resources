

- Quartz
- QCPlugInOutputImageProvider
-  supportedBufferPixelFormats() Deprecated

Instance Method

# supportedBufferPixelFormats()

Returns a list of pixel formats that are supported for rendering to a memory buffer.

macOS 10.4–10.15Deprecated

``` source
optional func supportedBufferPixelFormats() -> [Any]!
```

Deprecated

QuartzComposer API deprecated. (Define QC_SILENCE_DEPRECATION to silence these warnings)

## Return Value

A list of pixel formats, in order of preference, that the image can be rendered to in memory, or `nil` if the image provider does not support rendering to the CPU.

## See Also

### Providing Information About the Rendering Destination

func supportedRenderedTexturePixelFormats() -> [Any]!

Returns a list of pixel formats that are supported for rendering to an onscreen OpenGL context.

Deprecated

func canRender(withCGLContext: CGLContextObj!) -> Bool

Returns whether the image data can be rendered into the provided CGL context.

Deprecated

