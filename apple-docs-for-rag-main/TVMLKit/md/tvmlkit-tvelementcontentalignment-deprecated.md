

- TVMLKit
-  TVElementContentAlignment Deprecated

Enumeration

# TVElementContentAlignment

Location of items inside of an element on the vertical axis.

tvOS 9.0–18.0Deprecated

``` source
enum TVElementContentAlignment
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Constants

TVElementContentAlignmentUndefinded

The alignment has not been defined for the element.

case top

Items are aligned along the top of the element.

case center

Items are aligned in the center of the element.

case bottom

Items are aligned along the bottom of the element.

### Enumeration Cases

case undefined

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

