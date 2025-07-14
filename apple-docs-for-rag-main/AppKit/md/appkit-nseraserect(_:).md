

- AppKit
-  NSEraseRect(\_:) 

Function

# NSEraseRect(\_:)

Erases the specified rect by filling it with white.

macOS

``` source
func NSEraseRect(_ rect: NSRect)
```

## Parameters 

`rect`  

The rectangle (in the current coordinate system) defining the area to erase.

## Discussion

This function fills the specified rectangle with white. It does not alter the current color.

## See Also

### Drawing Rectangles

func NSDrawTiledRects(NSRect, NSRect, UnsafePointer&lt;NSRectEdge>, UnsafePointer&lt;CGFloat>, Int) -> NSRect

Draws rectangles with borders.

func NSDrawGroove(NSRect, NSRect)

Draws a gray-filled rectangle with a groove border.

