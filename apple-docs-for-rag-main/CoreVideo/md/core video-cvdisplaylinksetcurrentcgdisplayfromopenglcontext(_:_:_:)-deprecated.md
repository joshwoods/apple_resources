

- Core Video
-  CVDisplayLinkSetCurrentCGDisplayFromOpenGLContext(\_:\_:\_:) Deprecated

Function

# CVDisplayLinkSetCurrentCGDisplayFromOpenGLContext(\_:\_:\_:)

Selects the display link most optimal for the current renderer of an OpenGL context.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkSetCurrentCGDisplayFromOpenGLContext(
    _ displayLink: CVDisplayLink,
    _ cglContext: CGLContextObj,
    _ cglPixelFormat: CGLPixelFormatObj
) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLink`  

The display link whose current display is to be set.

`cglContext`  

The OpenGL context to retrieve the current renderer from.

`cglPixelFormat`  

The OpenGL pixel format used to create the passed-in OpenGL context.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

This function chooses the display with the lowest refresh rate.

## See Also

### Configuring Display Links

func CVDisplayLinkSetCurrentCGDisplay(CVDisplayLink, CGDirectDisplayID) -> CVReturn

Sets the current display of a display link.

Deprecated

func CVDisplayLinkSetOutputCallback(CVDisplayLink, CVDisplayLinkOutputCallback?, UnsafeMutableRawPointer?) -> CVReturn

Sets the renderer output callback function.

Deprecated

func CVDisplayLinkSetOutputHandler(CVDisplayLink, CVDisplayLinkOutputHandler) -> CVReturnDeprecated

typealias CVDisplayLinkOutputHandler

