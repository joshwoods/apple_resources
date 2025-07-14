

- RealityKit
- RealityViewDefaultPlaceholder
-  strikethrough(\_:pattern:color:) 

Instance Method

# strikethrough(\_:pattern:color:)

Applies a strikethrough to the text in this view.

RealityKitSwiftUIiOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

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

