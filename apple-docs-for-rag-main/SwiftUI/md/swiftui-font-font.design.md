

- SwiftUI
- Font
-  Font.Design 

Enumeration

# Font.Design

A design to use for fonts.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum Design
```

## Topics

### Getting font designs

case `default`

case monospaced

case rounded

case serif

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Getting system fonts

static func system(Font.TextStyle, design: Font.Design?, weight: Font.Weight?) -> Font

Gets a system font that uses the specified style, design, and weight.

static func system(size: CGFloat, weight: Font.Weight?, design: Font.Design?) -> Font

Specifies a system font to use, along with the style, weight, and any design parameters you want applied to the text.

enum TextStyle

A dynamic text style to use for fonts.

struct Weight

A weight to use for fonts.

