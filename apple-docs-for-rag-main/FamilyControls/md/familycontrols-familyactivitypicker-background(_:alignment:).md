

- FamilyControls
- FamilyActivityPicker
-  background(\_:alignment:) 

Instance Method

# background(\_:alignment:)

Layers the given view behind this view.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func background(
    _ background: Background,
    alignment: Alignment = .center
) -> some View where Background : View
```

## Parameters 

`background`  

The view to draw behind this view.

`alignment`  

The alignment with a default value of `Alignment/center` that you use to position the background view.

## Discussion

Use `background(_:alignment:)` when you need to place one view behind another, with the background view optionally aligned with a specified edge of the frontmost view.

The example below creates two views: the `Frontmost` view, and the `DiamondBackground` view. The `Frontmost` view uses the `DiamondBackground` view for the background of the image element inside the `Frontmost` view’s `VStack`.

```
struct DiamondBackground: View {
    var body: some View {
        VStack {
            Rectangle()
                .fill(.gray)
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

### Deprecated Layout Modifiers

func frame() -> some View

Positions this view within an invisible frame.

Deprecated

func edgesIgnoringSafeArea(Edge.Set) -> some View

Changes the view’s proposed area to extend outside the screen’s safe areas.

func overlay&lt;Overlay>(Overlay, alignment: Alignment) -> some View

Layers a secondary view in front of this view.

