

- Core Video
-  CVDisplayLinkSetOutputCallback(\_:\_:\_:) Deprecated

Function

# CVDisplayLinkSetOutputCallback(\_:\_:\_:)

Sets the renderer output callback function.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkSetOutputCallback(
    _ displayLink: CVDisplayLink,
    _ callback: CVDisplayLinkOutputCallback?,
    _ userInfo: UnsafeMutableRawPointer?
) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link whose output callback you want to set.

`callback`  

The callback function to set for this display link. See CVDisplayLinkOutputCallback for more information about implementing this function.

`userInfo`  

A pointer to user data.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

The display link invokes this callback whenever it wants you to output a frame.

## See Also

### Configuring Display Links

func CVDisplayLinkSetCurrentCGDisplay(CVDisplayLink, CGDirectDisplayID) -> CVReturn

Sets the current display of a display link.

Deprecated

func CVDisplayLinkSetCurrentCGDisplayFromOpenGLContext(CVDisplayLink, CGLContextObj, CGLPixelFormatObj) -> CVReturn

Selects the display link most optimal for the current renderer of an OpenGL context.

Deprecated

func CVDisplayLinkSetOutputHandler(CVDisplayLink, CVDisplayLinkOutputHandler) -> CVReturnDeprecated

typealias CVDisplayLinkOutputHandler

