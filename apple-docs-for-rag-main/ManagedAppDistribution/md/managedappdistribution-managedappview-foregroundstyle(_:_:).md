

- ManagedAppDistribution
- ManagedAppView
-  foregroundStyle(\_:\_:) 

Instance Method

# foregroundStyle(\_:\_:)

Sets the primary and secondary levels of the foreground style in the child view.

ManagedAppDistributionSwiftUIiOS 15.0+iPadOS 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func foregroundStyle(
    _ primary: S1,
    _ secondary: S2
) -> some View where S1 : ShapeStyle, S2 : ShapeStyle
```

## Parameters 

`primary`  

The primary color or pattern to use when filling in the foreground elements. To indicate a specific value, use `Color` or `ShapeStyle/image(_:sourceRect:scale:)`, or one of the gradient types, like `ShapeStyle/linearGradient(colors:startPoint:endPoint:)`. To set a style that’s relative to the containing view’s style, use one of the semantic styles, like `ShapeStyle/primary`.

`secondary`  

The secondary color or pattern to use when filling in the foreground elements.

## Return Value

A view that uses the given foreground styles.

## Discussion

SwiftUI uses these styles when rendering child views that don’t have an explicit rendering style, like images, text, shapes, and so on.

Symbol images within the view hierarchy use the `SymbolRenderingMode/palette` rendering mode when you apply this modifier, if you don’t explicitly specify another mode.

