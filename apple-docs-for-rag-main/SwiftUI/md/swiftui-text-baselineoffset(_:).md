

- SwiftUI
- Text
-  baselineOffset(\_:) 

Instance Method

# baselineOffset(\_:)

Sets the vertical offset for the text relative to its baseline.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func baselineOffset(_ baselineOffset: CGFloat) -> Text
```

## Parameters 

`baselineOffset`  

The amount to shift the text vertically (up or down) relative to its baseline.

## Return Value

Text that’s above or below its baseline.

## Discussion

Change the baseline offset to move the text in the view (in points) up or down relative to its baseline. The bounds of the view expand to contain the moved text.

```
HStack(alignment: .top) {
    Text("Hello")
        .baselineOffset(-10)
        .border(Color.red)
    Text("Hello")
        .border(Color.green)
    Text("Hello")
        .baselineOffset(10)
        .border(Color.blue)
}
.background(Color(white: 0.9))
```

By drawing a border around each text view, you can see how the text moves, and how that affects the view.

The first view, with a negative offset, grows downward to handle the lowered text. The last view, with a positive offset, grows upward. The enclosing HStack instance, shown in gray, ensures all the text views remain aligned at their top edge, regardless of the offset.

## See Also

### Styling the view’s text

func foregroundStyle&lt;S>(S) -> Text

Sets the style of the text displayed by this view.

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

enum Case

A scheme for transforming the capitalization of characters within text.

struct DateStyle

A predefined style used to display a `Date`.

