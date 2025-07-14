

- AppKit
- NSCursor
-  frameResize(position:directions:) 

Type Method

# frameResize(position:directions:)

Returns the cursor for resizing a rectangular frame from the specified edge or corner.

Mac Catalyst 18.0+macOS 15.0+

``` source
class func frameResize(
    position: NSCursor.FrameResizePosition,
    directions: NSCursor.FrameResizeDirection.Set
) -> NSCursor
```

## Parameters 

`position`  

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

`directions`  

The directions in which a rectangular frame can be resized. This must not be empty.

