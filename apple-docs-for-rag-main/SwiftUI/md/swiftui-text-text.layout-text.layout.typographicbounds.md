

- SwiftUI
- Text
- Text.Layout
-  Text.Layout.TypographicBounds 

Structure

# Text.Layout.TypographicBounds

The typographic bounds of an element in a text layout.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
@frozen
struct TypographicBounds
```

## Topics

### Initializers

init()

Initializes to an empty bounds with zero origin.

### Instance Properties

var ascent: CGFloat

The ascent of the element.

var descent: CGFloat

The descent of the element.

var leading: CGFloat

The leading of the element.

var origin: CGPoint

The position of the left edge of the element’s baseline, relative to the text view.

var rect: CGRect

Returns a rectangle encapsulating the bounds.

var width: CGFloat

The width of the element.

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Sendable

