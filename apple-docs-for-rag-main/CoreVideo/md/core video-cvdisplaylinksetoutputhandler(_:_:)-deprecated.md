

- Core Video
-  CVDisplayLinkSetOutputHandler(\_:\_:) Deprecated

Function

# CVDisplayLinkSetOutputHandler(\_:\_:)

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkSetOutputHandler(
    _ displayLink: CVDisplayLink,
    _ handler: @escaping CVDisplayLinkOutputHandler
) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

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

typealias CVDisplayLinkOutputHandler

