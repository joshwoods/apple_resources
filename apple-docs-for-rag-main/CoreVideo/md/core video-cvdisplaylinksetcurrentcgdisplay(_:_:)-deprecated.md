

- Core Video
-  CVDisplayLinkSetCurrentCGDisplay(\_:\_:) Deprecated

Function

# CVDisplayLinkSetCurrentCGDisplay(\_:\_:)

Sets the current display of a display link.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkSetCurrentCGDisplay(
    _ displayLink: CVDisplayLink,
    _ displayID: CGDirectDisplayID
) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link whose display you want to set.

`displayID`  

The ID of the display to be set.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

Although it is safe to call this function on a running display link, a discontinuity may appear in the video timestamp.

## See Also

### Configuring Display Links

func CVDisplayLinkSetCurrentCGDisplayFromOpenGLContext(CVDisplayLink, CGLContextObj, CGLPixelFormatObj) -> CVReturn

Selects the display link most optimal for the current renderer of an OpenGL context.

Deprecated

func CVDisplayLinkSetOutputCallback(CVDisplayLink, CVDisplayLinkOutputCallback?, UnsafeMutableRawPointer?) -> CVReturn

Sets the renderer output callback function.

Deprecated

func CVDisplayLinkSetOutputHandler(CVDisplayLink, CVDisplayLinkOutputHandler) -> CVReturnDeprecated

typealias CVDisplayLinkOutputHandler

