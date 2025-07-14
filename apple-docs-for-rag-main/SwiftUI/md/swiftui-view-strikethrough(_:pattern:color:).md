

- SwiftUI
- View
-  strikethrough(\_:pattern:color:) 

Instance Method

# strikethrough(\_:pattern:color:)

Applies a strikethrough to the text in this view.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
nonisolated
func strikethrough(
    _ isActive: Bool = true,
    pattern: Text.LineStyle.Pattern = .solid,
    color: Color? = nil
) -> some View
```

## Parameters 

`isActive`  

A Boolean value that indicates whether strikethrough is added. The default value is `true`.

`pattern`  

The pattern of the line. The default value is `solid`.

`color`  

The color of the strikethrough. If `color` is `nil`, the strikethrough uses the default foreground color.

## Return Value

A view where text has a line through its center.

## See Also

### Controlling text style

func bold(Bool) -> some View

Applies a bold font weight to the text in this view.

func italic(Bool) -> some View

Applies italics to the text in this view.

func underline(Bool, pattern: Text.LineStyle.Pattern, color: Color?) -> some View

Applies an underline to the text in this view.

func textCase(Text.Case?) -> some View

Sets a transform for the case of the text contained in this view when displayed.

var textCase: Text.Case?

A stylistic override to transform the case of `Text` when displayed, using the environment’s locale.

func monospaced(Bool) -> some View

Modifies the fonts of all child views to use the fixed-width variant of the current font, if possible.

func monospacedDigit() -> some View

Modifies the fonts of all child views to use fixed-width digits, if possible, while leaving other characters proportionally spaced.

