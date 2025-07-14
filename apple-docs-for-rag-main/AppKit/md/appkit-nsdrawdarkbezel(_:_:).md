

- AppKit
-  NSDrawDarkBezel(\_:\_:) 

Function

# NSDrawDarkBezel(\_:\_:)

Draws a dark gray-filled rectangle with a bezel border.

macOS

``` source
func NSDrawDarkBezel(
    _ rect: NSRect,
    _ clipRect: NSRect
)
```

## Parameters 

`rect`  

The bounding rectangle (in the current coordinate system) in which to draw. Only those parts of `aRect` that lie within the `clipRect` are actually drawn.

`clipRect`  

The clipping rectangle to use during drawing.

## See Also

### Related Documentation

func NSDrawTiledRects(NSRect, NSRect, UnsafePointer&lt;NSRectEdge>, UnsafePointer&lt;CGFloat>, Int) -> NSRect

Draws rectangles with borders.

### Drawing Bezels

func NSDrawGrayBezel(NSRect, NSRect)

Draws a gray-filled rectangle with a bezel border.

func NSDrawLightBezel(NSRect, NSRect)

Draws a white-filled rectangle with a bezel border.

func NSDrawWhiteBezel(NSRect, NSRect)

Draws a white-filled rectangle with a bezel border.

