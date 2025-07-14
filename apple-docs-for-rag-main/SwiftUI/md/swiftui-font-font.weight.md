

- SwiftUI
- Font
-  Font.Weight 

Structure

# Font.Weight

A weight to use for fonts.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
@frozen
struct Weight
```

## Topics

### Getting font weights

static let black: Font.Weight

static let bold: Font.Weight

static let heavy: Font.Weight

static let light: Font.Weight

static let medium: Font.Weight

static let regular: Font.Weight

static let semibold: Font.Weight

static let thin: Font.Weight

static let ultraLight: Font.Weight

## Relationships

### Conforms To

- BitwiseCopyable
- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Getting system fonts

static func system(Font.TextStyle, design: Font.Design?, weight: Font.Weight?) -> Font

Gets a system font that uses the specified style, design, and weight.

static func system(size: CGFloat, weight: Font.Weight?, design: Font.Design?) -> Font

Specifies a system font to use, along with the style, weight, and any design parameters you want applied to the text.

enum Design

A design to use for fonts.

enum TextStyle

A dynamic text style to use for fonts.

