

- SwiftUI
- PointerStyle
-  frameResize(position:directions:) 

Type Method

# frameResize(position:directions:)

The pointer style for resizing a rectangular frame from a specific edge or corner.

macOS 15.0+

``` source
static func frameResize(
    position: FrameResizePosition,
    directions: FrameResizeDirection.Set = .all
) -> PointerStyle
```

## Parameters 

`position`  

The position along the perimeter of the frame (its edges and corners) from which it’s resized.

`directions`  

The directions in which the frame can be resized.

