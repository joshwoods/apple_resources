

- SwiftUI
- View
-  background(\_:alignment:) Deprecated

Instance Method

# background(\_:alignment:)

Layers the given view behind this view.

iOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0–18.4DeprecatedvisionOS 1.0–2.4DeprecatedwatchOS 6.0–11.4Deprecated

``` source
nonisolated
func background(
    _ background: Background,
    alignment: Alignment = .center
) -> some View where Background : View
```

Deprecated

Use background(alignment:content:) instead.

## Parameters 

`background`  

The view to draw behind this view.

`alignment`  

The alignment with a default value of center that you use to position the background view.

## Mentioned in 

Adding a background to your view

Building layouts with stack views

## Discussion

Use `background(_:alignment:)` when you need to place one view behind another, with the background view optionally aligned with a specified edge of the frontmost view.

The example below creates two views: the `Frontmost` view, and the `DiamondBackground` view. The `Frontmost` view uses the `DiamondBackground` view for the background of the image element inside the `Frontmost` view’s VStack.

```
struct DiamondBackground: View {
    var body: some View {
        VStack {
            Rectangle()
                .fill(Color.gray)
                .frame(width: 250, height: 250, alignment: .center)
                .rotationEffect(.degrees(45.0))
        }
    }
}

struct Frontmost: View {
    var body: some View {
        VStack {
            Image(systemName: "folder")
                .font(.system(size: 128, weight: .ultraLight))
                .background(DiamondBackground())
        }
    }
}
```

## See Also

### Appearance modifiers

func colorScheme(ColorScheme) -> some View

Sets this view’s color scheme.

Deprecated

func listRowPlatterColor(Color?) -> some View

Sets the color that the system applies to the row background when this view is placed in a list.

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

