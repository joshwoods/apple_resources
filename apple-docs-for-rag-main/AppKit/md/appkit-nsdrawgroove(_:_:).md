

- AppKit
-  NSDrawGroove(\_:\_:) 

Function

# NSDrawGroove(\_:\_:)

Draws a gray-filled rectangle with a groove border.

macOS

``` source
func NSDrawGroove(
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

### Drawing Rectangles

func NSEraseRect(NSRect)

Erases the specified rect by filling it with white.

func NSDrawTiledRects(NSRect, NSRect, UnsafePointer&lt;NSRectEdge>, UnsafePointer&lt;CGFloat>, Int) -> NSRect

Draws rectangles with borders.

