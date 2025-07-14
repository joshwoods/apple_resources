

- RealityKit
- RealityViewAttachmentBuilderContent
-  colorScheme(\_:) 

Instance Method

# colorScheme(\_:)

Sets this view’s color scheme.

RealityKitSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0–2.4DeprecatedwatchOS 6.0+

``` source
nonisolated
func colorScheme(_ colorScheme: ColorScheme) -> some View
```

## Parameters 

`colorScheme`  

The color scheme for this view.

## Return Value

A view that sets this view’s color scheme.

## Discussion

Use `colorScheme(_:)` to set the color scheme for the view to which you apply it and any subviews. If you want to set the color scheme for all views in the presentation, use `View/preferredColorScheme(_:)` instead.

