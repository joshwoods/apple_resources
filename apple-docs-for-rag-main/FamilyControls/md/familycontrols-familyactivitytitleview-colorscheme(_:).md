

- FamilyControls
- FamilyActivityTitleView
-  colorScheme(\_:) 

Instance Method

# colorScheme(\_:)

Sets this view’s color scheme.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

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

