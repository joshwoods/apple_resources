

- Core Video
-  CVDisplayLinkCreateWithActiveCGDisplays(\_:) Deprecated

Function

# CVDisplayLinkCreateWithActiveCGDisplays(\_:)

Creates a display link capable of being used with all active displays.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkCreateWithActiveCGDisplays(_ displayLinkOut: UnsafeMutablePointer) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayLinkOut`  

On output, `displayLinkOut` points to the newly created display link.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

`CVDisplayLinkCreateWithActiveCGDisplays` determines the displays actively used by the host computer and creates a display link compatible with all of them. For most applications, calling this function is the most convenient way to create a display link. After creation, you can assign the display link to any active display by calling the CVDisplayLinkSetCurrentCGDisplay(_:_:) function.

## See Also

### Creating Display Links

func CVDisplayLinkCreateWithCGDisplay(CGDirectDisplayID, UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link for a single display.

Deprecated

func CVDisplayLinkCreateWithCGDisplays(UnsafeMutablePointer&lt;CGDirectDisplayID>, CFIndex, UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link for an array of displays.

Deprecated

func CVDisplayLinkCreateWithOpenGLDisplayMask(CGOpenGLDisplayMask, UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link from an OpenGL display mask.

Deprecated

