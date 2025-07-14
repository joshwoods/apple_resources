

- TVMLKit
-  TVElementAlignment Deprecated

Enumeration

# TVElementAlignment

Location of an item inside of an element on the horizontal axis.

tvOS 9.0–18.0Deprecated

``` source
enum TVElementAlignment
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Constants

case undefined

The alignment has not been defined for the item.

case left

The item is aligned along the left side of the containing element.

case center

The item is aligned in the center of the containing element.

case right

The item is aligned along the right of the containing element.

case leading

The item is aligned along the leading edge of the containing element.

case trailing

The item is aligned along the trailing edge of the containing element.

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

enum TVElementPosition

Location of an element relative to the screen or its containing element.

Deprecated

