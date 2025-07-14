

- Core Video
-  CVDisplayLinkCreateWithOpenGLDisplayMask(\_:\_:) Deprecated

Function

# CVDisplayLinkCreateWithOpenGLDisplayMask(\_:\_:)

Creates a display link from an OpenGL display mask.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkCreateWithOpenGLDisplayMask(
    _ mask: CGOpenGLDisplayMask,
    _ displayLinkOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`mask`  

The OpenGL display mask describing the available displays.

`displayLinkOut`  

On output, `displayLinkOut` points to the newly created display link.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

Using this function avoids having to call the Core Graphics function `CGOpenGLDisplayMaskToDisplayID`.

## See Also

### Creating Display Links

func CVDisplayLinkCreateWithCGDisplay(CGDirectDisplayID, UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link for a single display.

Deprecated

func CVDisplayLinkCreateWithCGDisplays(UnsafeMutablePointer&lt;CGDirectDisplayID>, CFIndex, UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link for an array of displays.

Deprecated

func CVDisplayLinkCreateWithActiveCGDisplays(UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link capable of being used with all active displays.

Deprecated

