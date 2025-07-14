

- SwiftUI
- Text
- Text.LineStyle
-  Text.LineStyle.Pattern 

Structure

# Text.LineStyle.Pattern

The pattern, that the line has.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Pattern
```

## Topics

### Getting line style patterns

static let solid: Text.LineStyle.Pattern

Draw a solid line.

static let dot: Text.LineStyle.Pattern

Draw a line of dots.

static let dash: Text.LineStyle.Pattern

Draw a line of dashes.

static let dashDot: Text.LineStyle.Pattern

static let dashDotDot: Text.LineStyle.Pattern

Draw a line of alternating dashes and two dots.

## Relationships

### Conforms To

- Sendable

## See Also

### Creating a text line style

init?(nsUnderlineStyle: NSUnderlineStyle)

Creates a `Text.LineStyle` from `NSUnderlineStyle`.

init(pattern: Text.LineStyle.Pattern, color: Color?)

Creates a line style.

