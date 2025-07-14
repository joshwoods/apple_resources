

- SwiftUI
- View
-  textCase(\_:) 

Instance Method

# textCase(\_:)

Sets a transform for the case of the text contained in this view when displayed.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
nonisolated
func textCase(_ textCase: Text.Case?) -> some View
```

## Parameters 

`textCase`  

One of the Text.Case enumerations; the default is `nil`.

## Return Value

A view that transforms the case of the text.

## Discussion

The default value is `nil`, displaying the text without any case changes.

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

var textCase: Text.Case?

A stylistic override to transform the case of `Text` when displayed, using the environment’s locale.

func monospaced(Bool) -> some View

Modifies the fonts of all child views to use the fixed-width variant of the current font, if possible.

func monospacedDigit() -> some View

Modifies the fonts of all child views to use fixed-width digits, if possible, while leaving other characters proportionally spaced.

