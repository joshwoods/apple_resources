

- FamilyControls
- FamilyActivityPicker
-  foregroundStyle(\_:\_:\_:) 

Instance Method

# foregroundStyle(\_:\_:\_:)

Sets the primary, secondary, and tertiary levels of the foreground style.

FamilyControlsSwiftUIiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+watchOS 8.0+

``` source
nonisolated
func foregroundStyle(
    _ primary: S1,
    _ secondary: S2,
    _ tertiary: S3
) -> some View where S1 : ShapeStyle, S2 : ShapeStyle, S3 : ShapeStyle
```

## Parameters 

`primary`  

The primary color or pattern to use when filling in the foreground elements. To indicate a specific value, use `Color` or `ShapeStyle/image(_:sourceRect:scale:)`, or one of the gradient types, like `ShapeStyle/linearGradient(colors:startPoint:endPoint:)`. To set a style that’s relative to the containing view’s style, use one of the semantic styles, like `ShapeStyle/primary`.

`secondary`  

The secondary color or pattern to use when filling in the foreground elements.

`tertiary`  

The tertiary color or pattern to use when filling in the foreground elements.

## Return Value

A view that uses the given foreground styles.

## Discussion

SwiftUI uses these styles when rendering child views that don’t have an explicit rendering style, like images, text, shapes, and so on.

Symbol images within the view hierarchy use the `SymbolRenderingMode/palette` rendering mode when you apply this modifier, if you don’t explicitly specify another mode.

## See Also

### Foreground Elements

func foregroundStyle&lt;S>(S) -> some View

Sets a view’s foreground elements to use a given style.

func foregroundStyle&lt;S1, S2>(S1, S2) -> some View

Sets the primary and secondary levels of the foreground style in the child view.

func foregroundColor(Color?) -> some View

Sets the color of the foreground elements displayed by this view.

func overlay&lt;S>(S, ignoresSafeAreaEdges: Edge.Set) -> some View

Layers the specified style in front of this view.

func overlay&lt;S, T>(S, in: T, fillStyle: FillStyle) -> some View

Layers a shape that you specify in front of this view.

