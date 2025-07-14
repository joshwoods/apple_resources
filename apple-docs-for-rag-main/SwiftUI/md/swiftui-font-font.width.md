

- SwiftUI
- Font
-  Font.Width 

Structure

# Font.Width

A width to use for fonts that have multiple widths.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
struct Width
```

## Topics

### Getting standard font widths

static let compressed: Font.Width

static let condensed: Font.Width

static let expanded: Font.Width

static let standard: Font.Width

### Creating an explicit font width

init(CGFloat)

### Accessing the width’s value

var value: CGFloat

## Relationships

### Conforms To

- Equatable
- Hashable
- Sendable

## See Also

### Styling a font

func bold() -> Font

Adds bold styling to the font.

func italic() -> Font

Adds italics to the font.

func monospaced() -> Font

Returns a fixed-width font from the same family as the base font.

func monospacedDigit() -> Font

Returns a modified font that uses fixed-width digits, while leaving other characters proportionally spaced.

func smallCaps() -> Font

Adjusts the font to enable all small capitals.

func lowercaseSmallCaps() -> Font

Adjusts the font to enable lowercase small capitals.

func uppercaseSmallCaps() -> Font

Adjusts the font to enable uppercase small capitals.

func weight(Font.Weight) -> Font

Sets the weight of the font.

func width(Font.Width) -> Font

Sets the width of the font.

func leading(Font.Leading) -> Font

Adjusts the line spacing of a font.

enum Leading

A line spacing adjustment that you can apply to a font.

