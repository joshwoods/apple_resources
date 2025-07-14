

- Core Video
-  CVDisplayLinkOutputHandler 

Type Alias

# CVDisplayLinkOutputHandler

Mac Catalyst 13.0+macOS 10.4+

``` source
typealias CVDisplayLinkOutputHandler = (CVDisplayLink, UnsafePointer, UnsafePointer, CVOptionFlags, UnsafeMutablePointer) -> CVReturn
```

## See Also

### Configuring Display Links

func CVDisplayLinkSetCurrentCGDisplay(CVDisplayLink, CGDirectDisplayID) -> CVReturn

Sets the current display of a display link.

Deprecated

func CVDisplayLinkSetCurrentCGDisplayFromOpenGLContext(CVDisplayLink, CGLContextObj, CGLPixelFormatObj) -> CVReturn

Selects the display link most optimal for the current renderer of an OpenGL context.

Deprecated

func CVDisplayLinkSetOutputCallback(CVDisplayLink, CVDisplayLinkOutputCallback?, UnsafeMutableRawPointer?) -> CVReturn

Sets the renderer output callback function.

Deprecated

func CVDisplayLinkSetOutputHandler(CVDisplayLink, CVDisplayLinkOutputHandler) -> CVReturnDeprecated

