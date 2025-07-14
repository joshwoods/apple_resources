

- SwiftUI
- Text
-  tracking(\_:) 

Instance Method

# tracking(\_:)

Sets the tracking for the text.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func tracking(_ tracking: CGFloat) -> Text
```

## Parameters 

`tracking`  

The amount of additional space, in points, that the view should add to each character cluster after layout. Value of `0` sets the tracking to the system default value.

## Return Value

Text with the specified amount of tracking.

## Discussion

Tracking adds space, measured in points, between the characters in the text view. A positive value increases the spacing between characters, while a negative value brings the characters closer together.

```
VStack(alignment: .leading) {
    Text("ABCDEF").tracking(-3)
    Text("ABCDEF")
    Text("ABCDEF").tracking(3)
}
```

The code above uses an unusually large amount of tracking to make it easy to see the effect.

The effect of tracking resembles that of the kerning(_:) modifier, but adds or removes trailing whitespace, rather than changing character offsets. Also, using any nonzero amount of tracking disables nonessential ligatures, whereas kerning attempts to maintain ligatures.

Important

If you add both the tracking(_:) and kerning(_:) modifiers to a view, the view applies the tracking and ignores the kerning.

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

func baselineOffset(CGFloat) -> Text

Sets the vertical offset for the text relative to its baseline.

enum Case

A scheme for transforming the capitalization of characters within text.

struct DateStyle

A predefined style used to display a `Date`.

