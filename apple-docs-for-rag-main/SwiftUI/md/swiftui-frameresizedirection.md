

- SwiftUI
-  FrameResizeDirection 

Enumeration

# FrameResizeDirection

The direction in which a rectangular frame can be resized.

macOS 15.0+

``` source
@frozen
enum FrameResizeDirection
```

## Topics

### Structures

struct Set

An efficient set of frame resize directions.

### Enumeration Cases

case inward

Indicates that the frame can be resized inwards to be smaller.

case outward

Indicates that the frame can be resized outwards to be larger.

## Relationships

### Conforms To

- BitwiseCopyable
- CaseIterable
- Copyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Modifying pointer appearance

func pointerStyle(PointerStyle?) -> some View

Sets the pointer style to display when the pointer is over the view.

struct PointerStyle

A style describing the appearance of the pointer (also called a cursor) when it’s hovered over a view.

func pointerVisibility(Visibility) -> some View

Sets the visibility of the pointer when it’s over the view.

enum HorizontalDirection

A direction on the horizontal axis.

enum VerticalDirection

A direction on the horizontal axis.

enum FrameResizePosition

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

