

- SwiftUI
- Font
-  uppercaseSmallCaps() 

Instance Method

# uppercaseSmallCaps()

Adjusts the font to enable uppercase small capitals.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
func uppercaseSmallCaps() -> Font
```

## Discussion

This feature turns capital characters into small capitals. It is generally used for words which would otherwise be set in all caps, such as acronyms, but which are desired in small-cap form to avoid disrupting the flow of text.

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

func weight(Font.Weight) -> Font

Sets the weight of the font.

func width(Font.Width) -> Font

Sets the width of the font.

struct Width

A width to use for fonts that have multiple widths.

func leading(Font.Leading) -> Font

Adjusts the line spacing of a font.

enum Leading

A line spacing adjustment that you can apply to a font.

