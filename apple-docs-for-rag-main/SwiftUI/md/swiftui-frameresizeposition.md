

- SwiftUI
-  FrameResizePosition 

Enumeration

# FrameResizePosition

The position along the perimeter of a rectangular frame (its edges and corners) from which it’s resized.

macOS 15.0+

``` source
@frozen
enum FrameResizePosition
```

## Topics

### Enumeration Cases

case bottom

The bottom edge of the frame.

case bottomLeading

The bottom leading corner of the frame.

case bottomTrailing

The bottom trailing corner of the frame.

case leading

The leading edge of the frame.

case top

The top edge of the frame.

case topLeading

The top leading corner of the frame.

case topTrailing

The top trailing edge of the frame.

case trailing

The trailing edge of the frame.

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

enum FrameResizeDirection

The direction in which a rectangular frame can be resized.

