

- FamilyControls
- FamilyActivityPicker
-  overlay(\_:alignment:) 

Instance Method

# overlay(\_:alignment:)

Layers a secondary view in front of this view.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func overlay(
    _ overlay: Overlay,
    alignment: Alignment = .center
) -> some View where Overlay : View
```

## Parameters 

`overlay`  

The view to layer in front of this view.

`alignment`  

The alignment for `overlay` in relation to this view.

## Return Value

A view that layers `overlay` in front of the view.

## Discussion

When you apply an overlay to a view, the original view continues to provide the layout characteristics for the resulting view. In the following example, the heart image is shown overlaid in front of, and aligned to the bottom of the folder image.

```
Image(systemName: "folder")
    .font(.system(size: 55, weight: .thin))
    .overlay(Text("❤️"), alignment: .bottom)
```

## See Also

### Deprecated Layout Modifiers

func frame() -> some View

Positions this view within an invisible frame.

Deprecated

func edgesIgnoringSafeArea(Edge.Set) -> some View

Changes the view’s proposed area to extend outside the screen’s safe areas.

func background&lt;Background>(Background, alignment: Alignment) -> some View

Layers the given view behind this view.

