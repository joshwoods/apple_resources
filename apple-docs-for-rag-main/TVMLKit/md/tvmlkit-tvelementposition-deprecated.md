

- TVMLKit
-  TVElementPosition Deprecated

Enumeration

# TVElementPosition

Location of an element relative to the screen or its containing element.

tvOS 9.0–18.0Deprecated

``` source
enum TVElementPosition
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Constants

case undefined

The position has not been defined.

case center

Position the element in the center of its containing element.

case top

Position the element at the top of the containing element.

case bottom

Position the element at the bottom of the containing element.

case left

Position the element along the left side of the containing element.

case right

Position the element along the right side of the containing element.

case topLeft

Position the element in the top-left of the containing element.

case topRight

Position the element in the top-right of the containing element.

case bottomLeft

Position the element in the bottom-left of the containing element.

case bottomRight

Position the element in the bottom-right of the containing element.

case header

Position the element in the header area of the containing element.

case footer

Position the element in the footer area of the containing element.

case leading

Position the element in the leading edge of the containing element.

case trailing

Position the element in the trailing edge of the containing element.

case topLeading

Position the element in the top-leading edge of the containing element.

case topTrailing

Position the element in the top-trailing edge of the containing element.

case bottomLeading

Position the element in the bottom-leading edge of the containing element.

case bottomTrailing

Position the element in the bottom-trailing edge of the containing element.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Aligning and Positioning an Element

var alignment: TVElementAlignment

A value indicating how an item is aligned inside of an element.

Deprecated

enum TVElementAlignment

Location of an item inside of an element on the horizontal axis.

Deprecated

var contentAlignment: TVElementContentAlignment

A value indicating how items inside of an element are aligned.

Deprecated

enum TVElementContentAlignment

Location of items inside of an element on the vertical axis.

Deprecated

var focusMargin: UIEdgeInsets

The amount of space, in pixels, a custom cell requires when it comes into focus.

Deprecated

var interitemSpacing: CGFloat

The spacing, in pixels, between items inside of an element.

Deprecated

var margin: UIEdgeInsets

The amount of space, in pixels, between the element and other elements.

Deprecated

var padding: UIEdgeInsets

The amount of space, in pixels, between the border and the contents of the element.

Deprecated

var position: TVElementPosition

A value indicating the position of the element relative to the screen or its containing element.

Deprecated

