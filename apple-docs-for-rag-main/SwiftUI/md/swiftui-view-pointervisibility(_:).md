

- SwiftUI
- View
-  pointerVisibility(\_:) 

Instance Method

# pointerVisibility(\_:)

Sets the visibility of the pointer when it’s over the view.

macOS 15.0+

``` source
nonisolated
func pointerVisibility(_ visibility: Visibility) -> some View
```

## Parameters 

`visibility`  

The pointer visibility to apply.

## Return Value

A view that changes the visibility of the pointer when hovered.

## See Also

### Modifying pointer appearance

func pointerStyle(PointerStyle?) -> some View

Sets the pointer style to display when the pointer is over the view.

struct PointerStyle

A style describing the appearance of the pointer (also called a cursor) when it’s hovered over a view.

enum HorizontalDirection

A direction on the horizontal axis.

enum VerticalDirection

A direction on the horizontal axis.

enum FrameResizePosition

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

enum FrameResizeDirection

The direction in which a rectangular frame can be resized.

