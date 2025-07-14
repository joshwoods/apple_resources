

- SwiftUI
- View
-  colorScheme(\_:) Deprecated

Instance Method

# colorScheme(\_:)

Sets this view’s color scheme.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func colorScheme(_ colorScheme: ColorScheme) -> some View
```

Deprecated

Use preferredColorScheme(_:) instead.

## Parameters 

`colorScheme`  

The color scheme for this view.

## Return Value

A view that sets this view’s color scheme.

## Discussion

Use `colorScheme(_:)` to set the color scheme for the view to which you apply it and any subviews.

## See Also

### Appearance modifiers

func listRowPlatterColor(Color?) -> some View

Sets the color that the system applies to the row background when this view is placed in a list.

Deprecated

func background&lt;Background>(Background, alignment: Alignment) -> some View

Layers the given view behind this view.

Deprecated

func overlay&lt;Overlay>(Overlay, alignment: Alignment) -> some View

Layers a secondary view in front of this view.

Deprecated

func foregroundColor(Color?) -> some View

Sets the color of the foreground elements displayed by this view.

Deprecated

func complicationForeground() -> some View

Promotes this view to the foreground in a complication.

Deprecated

