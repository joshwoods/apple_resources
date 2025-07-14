

- Core Video
-  CVDisplayLinkCreateWithCGDisplay(\_:\_:) Deprecated

Function

# CVDisplayLinkCreateWithCGDisplay(\_:\_:)

Creates a display link for a single display.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkCreateWithCGDisplay(
    _ displayID: CGDirectDisplayID,
    _ displayLinkOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayID`  

The Core Graphics ID of the target display.

`displayLinkOut`  

On output, `displayLinkOut` points to the newly created display link.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

Use this call to create a display link for a single display. For more information on the display identifier type, see CGDirectDisplayID.

## See Also

### Creating Display Links

func CVDisplayLinkCreateWithCGDisplays(UnsafeMutablePointer&lt;CGDirectDisplayID>, CFIndex, UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link for an array of displays.

Deprecated

func CVDisplayLinkCreateWithActiveCGDisplays(UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link capable of being used with all active displays.

Deprecated

func CVDisplayLinkCreateWithOpenGLDisplayMask(CGOpenGLDisplayMask, UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link from an OpenGL display mask.

Deprecated

