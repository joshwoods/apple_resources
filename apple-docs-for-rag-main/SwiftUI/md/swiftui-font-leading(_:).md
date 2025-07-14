

- SwiftUI
- Font
-  leading(\_:) 

Instance Method

# leading(\_:)

Adjusts the line spacing of a font.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
func leading(_ leading: Font.Leading) -> Font
```

## Parameters 

`leading`  

The line spacing adjustment to apply.

## Return Value

A modified font that uses the specified line spacing, or the original font if it doesn’t support line spacing adjustments.

## Discussion

You can change a font’s line spacing while maintaining other characteristics of the font by applying this modifier. For example, you can decrease spacing of the body font by applying the Font.Leading.tight value to it:

```
let myFont = Font.body.leading(.tight)
```

The availability of leading adjustments depends on the font. For some fonts, the modifier has no effect and returns the original font.

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

enum Leading

A line spacing adjustment that you can apply to a font.

