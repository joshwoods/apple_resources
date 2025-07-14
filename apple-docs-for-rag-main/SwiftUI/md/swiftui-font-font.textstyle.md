

- SwiftUI
- Font
-  Font.TextStyle 

Enumeration

# Font.TextStyle

A dynamic text style to use for fonts.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
enum TextStyle
```

## Topics

### Getting font text styles

case extraLargeTitle2

The font used for second level extra large titles.

case extraLargeTitle

The font used for extra large titles.

case largeTitle

The font style for large titles.

case title

The font used for first level hierarchical headings.

case title2

The font used for second level hierarchical headings.

case title3

The font used for third level hierarchical headings.

case headline

The font used for headings.

case subheadline

The font used for subheadings.

case body

The font used for body text.

case callout

The font used for callouts.

case caption

The font used for standard captions.

case caption2

The font used for alternate captions.

case footnote

The font used in footnotes.

## Relationships

### Conforms To

- CaseIterable
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

struct Weight

A weight to use for fonts.

