

- SwiftUI
- View
-  overlay(\_:alignment:) Deprecated

Instance Method

# overlay(\_:alignment:)

Layers a secondary view in front of this view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func overlay(
    _ overlay: Overlay,
    alignment: Alignment = .center
) -> some View where Overlay : View
```

Deprecated

Use overlay(alignment:content:) instead.

## Parameters 

`overlay`  

The view to layer in front of this view.

`alignment`  

The alignment for `overlay` in relation to this view.

## Return Value

A view that layers `overlay` in front of the view.

## Mentioned in 

Building layouts with stack views

## Discussion

When you apply an overlay to a view, the original view continues to provide the layout characteristics for the resulting view. In the following example, the heart image is shown overlaid in front of, and aligned to the bottom of the folder image.

```
Image(systemName: "folder")
    .font(.system(size: 55, weight: .thin))
    .overlay(Text("❤️"), alignment: .bottom)
```

## See Also

### Appearance modifiers

func colorScheme(ColorScheme) -> some View

Sets this view’s color scheme.

Deprecated

func listRowPlatterColor(Color?) -> some View

Sets the color that the system applies to the row background when this view is placed in a list.

Deprecated

func background&lt;Background>(Background, alignment: Alignment) -> some View

Layers the given view behind this view.

Deprecated

func foregroundColor(Color?) -> some View

Sets the color of the foreground elements displayed by this view.

Deprecated

func complicationForeground() -> some View

Promotes this view to the foreground in a complication.

Deprecated

