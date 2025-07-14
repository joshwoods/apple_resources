

- SwiftUI
- View
-  monospacedDigit() 

Instance Method

# monospacedDigit()

Modifies the fonts of all child views to use fixed-width digits, if possible, while leaving other characters proportionally spaced.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
nonisolated
func monospacedDigit() -> some View
```

## Return Value

A view whose child views’ fonts use fixed-width numeric characters, while leaving other characters proportionally spaced.

## Discussion

Using fixed-width digits allows you to easily align numbers of the same size in a table-like arrangement. This feature is also known as “tabular figures” or “tabular numbers.”

This modifier only affects numeric characters, and leaves all other characters unchanged.

The following example shows the effect of `monospacedDigit()` on multiple child views. The example consists of two VStack views inside an HStack. Each `VStack` contains two Button views, with the second `VStack` applying the `monospacedDigit()` modifier to its contents. As a result, the digits in the buttons in the trailing `VStack` are the same width, which in turn gives the buttons equal widths.

```
var body: some View {
    HStack(alignment: .top) {
        VStack(alignment: .leading) {
            Button("Delete 111 messages") {}
            Button("Delete 222 messages") {}
        }
        VStack(alignment: .leading) {
            Button("Delete 111 messages") {}
            Button("Delete 222 messages") {}
        }
        .monospacedDigit()
    }
    .padding()
    .navigationTitle("monospacedDigit() Child Views")
}
```

If a child view’s base font doesn’t support fixed-width digits, the font remains unchanged.

## See Also

### Controlling text style

func bold(Bool) -> some View

Applies a bold font weight to the text in this view.

func italic(Bool) -> some View

Applies italics to the text in this view.

func underline(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> some View

Applies an underline to the text in this view.

func strikethrough(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> some View

Applies a strikethrough to the text in this view.

func textCase(Text.Case?) -> some View

Sets a transform for the case of the text contained in this view when displayed.

var textCase: Text.Case?

A stylistic override to transform the case of `Text` when displayed, using the environment’s locale.

func monospaced(Bool) -> some View

Modifies the fonts of all child views to use the fixed-width variant of the current font, if possible.

