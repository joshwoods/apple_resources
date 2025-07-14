

- SwiftUI
- View
-  monospaced(\_:) 

Instance Method

# monospaced(\_:)

Modifies the fonts of all child views to use the fixed-width variant of the current font, if possible.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func monospaced(_ isActive: Bool = true) -> some View
```

## Return Value

A view whose child views’ fonts use fixed-width characters, while leaving other characters proportionally spaced.

## Discussion

If a child view’s base font doesn’t support fixed-width, the font remains unchanged.

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

func monospacedDigit() -> some View

Modifies the fonts of all child views to use fixed-width digits, if possible, while leaving other characters proportionally spaced.

