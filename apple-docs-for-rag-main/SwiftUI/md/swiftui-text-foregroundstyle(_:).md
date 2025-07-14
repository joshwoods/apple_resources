

- SwiftUI
- Text
-  foregroundStyle(\_:) 

Instance Method

# foregroundStyle(\_:)

Sets the style of the text displayed by this view.

iOS 17.0+iPadOS 17.0+Mac Catalyst 17.0+macOS 14.0+tvOS 17.0+visionOS 1.0+watchOS 10.0+

``` source
nonisolated
func foregroundStyle(_ style: S) -> Text where S : ShapeStyle
```

## Parameters 

`style`  

The style to use when displaying this text.

## Return Value

A text view that uses the color value you supply.

## Discussion

Use this method to change the rendering style of the text rendered by a text view.

For example, you can display the names of the colors red, green, and blue in their respective colors:

```
HStack {
    Text("Red").foregroundStyle(.red)
    Text("Green").foregroundStyle(.green)
    Text("Blue").foregroundStyle(.blue)
}
```

## See Also

### Styling the view’s text

func bold() -> Text

Applies a bold font weight to the text.

func bold(Bool) -> Text

Applies a bold font weight to the text.

func italic() -> Text

Applies italics to the text.

func italic(Bool) -> Text

Applies italics to the text.

func strikethrough(Bool, color: Color?) -> Text

Applies a strikethrough to the text.

func strikethrough(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> Text

Applies a strikethrough to the text.

func underline(Bool, color: Color?) -> Text

Applies an underline to the text.

func underline(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> Text

Applies an underline to the text.

func monospaced(Bool) -> Text

Modifies the font of the text to use the fixed-width variant of the current font, if possible.

func monospacedDigit() -> Text

Modifies the text view’s font to use fixed-width digits, while leaving other characters proportionally spaced.

func kerning(CGFloat) -> Text

Sets the spacing, or kerning, between characters.

func tracking(CGFloat) -> Text

Sets the tracking for the text.

func baselineOffset(CGFloat) -> Text

Sets the vertical offset for the text relative to its baseline.

enum Case

A scheme for transforming the capitalization of characters within text.

struct DateStyle

A predefined style used to display a `Date`.

