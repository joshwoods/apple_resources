

- SwiftUI
- Text
-  monospacedDigit() 

Instance Method

# monospacedDigit()

Modifies the text view’s font to use fixed-width digits, while leaving other characters proportionally spaced.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func monospacedDigit() -> Text
```

## Return Value

A text view with a modified font that uses fixed-width numeric characters, while leaving other characters proportionally spaced.

## Discussion

This modifier only affects numeric characters, and leaves all other characters unchanged.

The following example shows the effect of `monospacedDigit()` on a text view. It arranges two text views in a VStack, each displaying a formatted date that contains many instances of the character 1. The second text view uses the `monospacedDigit()`. Because 1 is usually a narrow character in proportional fonts, applying the modifier widens all of the 1s, and the text view as a whole. The non-digit characters in the text view remain unaffected.

```
let myDate = DateComponents(
    calendar: Calendar(identifier: .gregorian),
    timeZone: TimeZone(identifier: "EST"),
    year: 2011,
    month: 1,
    day: 11,
    hour: 11,
    minute: 11
).date!

var body: some View {
    VStack(alignment: .leading) {
        Text(myDate.formatted(date: .long, time: .complete))
            .font(.system(size: 20))
        Text(myDate.formatted(date: .long, time: .complete))
            .font(.system(size: 20))
            .monospacedDigit()
    }
    .padding()
    .navigationTitle("monospacedDigit() Modifier")
}
```

If the base font of the text view doesn’t support fixed-width digits, the font remains unchanged.

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

