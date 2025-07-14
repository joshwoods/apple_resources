

- SwiftUI
- Font
-  Font.Leading 

Enumeration

# Font.Leading

A line spacing adjustment that you can apply to a font.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum Leading
```

## Overview

Apply one of the `Leading` values to a font using the leading(_:) method to increase or decrease the line spacing.

## Topics

### Getting leading line spacing options

case standard

The font’s default line spacing.

case loose

Increased line spacing.

case tight

Reduced line spacing.

## Relationships

### Conforms To

- Copyable
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

struct Width

A width to use for fonts that have multiple widths.

func leading(Font.Leading) -> Font

Adjusts the line spacing of a font.

