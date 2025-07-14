

- Core Video
-  CVDisplayLinkCreateWithCGDisplays(\_:\_:\_:) Deprecated

Function

# CVDisplayLinkCreateWithCGDisplays(\_:\_:\_:)

Creates a display link for an array of displays.

Mac Catalyst 13.1–18.0DeprecatedmacOS 10.4–15.0Deprecated

``` source
func CVDisplayLinkCreateWithCGDisplays(
    _ displayArray: UnsafeMutablePointer,
    _ count: CFIndex,
    _ displayLinkOut: UnsafeMutablePointer
) -> CVReturn
```

Deprecated

use NSView.displayLink(target:selector:), NSWindow.displayLink(target:selector:), or NSScreen.displayLink(target:selector:)

## Parameters 

`displayArray`  

A pointer to an array of Core Graphics display IDs representing all the active monitors you want to use with this display link.

`count`  

The number of displays in the display array.

`displayLinkOut`  

On output, `displayLinkOut` points to the newly created display link.

## Return Value

A Core Video result code. See Core Video Constants for possible values.

## Discussion

Use this call to create a display link for a set of displays identified by the Core Graphics display IDs. For more information on the display identifier type, see CGDirectDisplayID.

## See Also

### Creating Display Links

func CVDisplayLinkCreateWithCGDisplay(CGDirectDisplayID, UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link for a single display.

Deprecated

func CVDisplayLinkCreateWithActiveCGDisplays(UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link capable of being used with all active displays.

Deprecated

func CVDisplayLinkCreateWithOpenGLDisplayMask(CGOpenGLDisplayMask, UnsafeMutablePointer&lt;CVDisplayLink?>) -> CVReturn

Creates a display link from an OpenGL display mask.

Deprecated

