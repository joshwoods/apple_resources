

- FamilyControls
- FamilyActivityPicker
-  edgesIgnoringSafeArea(\_:) 

Instance Method

# edgesIgnoringSafeArea(\_:)

Changes the view’s proposed area to extend outside the screen’s safe areas.

FamilyControlsSwiftUIiOS 13.0–18.4DeprecatediPadOS 13.0–18.4DeprecatedMac Catalyst 13.0–18.4DeprecatedmacOS 10.15–15.4DeprecatedtvOS 13.0+visionOS 1.0+watchOS 6.0–11.4Deprecated

``` source
nonisolated
func edgesIgnoringSafeArea(_ edges: Edge.Set) -> some View
```

## Parameters 

`edges`  

The set of the edges in which to expand the size requested for this view.

## Return Value

A view that may extend outside of the screen’s safe area on the edges specified by `edges`.

## Discussion

Use `edgesIgnoringSafeArea(_:)` to change the area proposed for this view so that — were the proposal accepted — this view could extend outside the safe area to the bounds of the screen for the specified edges.

For example, you can propose that a text view ignore the safe area’s top inset:

```
VStack {
    Text("This text is outside of the top safe area.")
        .edgesIgnoringSafeArea([.top])
        .border(Color.purple)
    Text("This text is inside VStack.")
        .border(Color.yellow)
}
.border(Color.gray)
```

Depending on the surrounding view hierarchy, SwiftUI may not honor an `edgesIgnoringSafeArea(_:)` request. This can happen, for example, if the view is inside a container that respects the screen’s safe area. In that case you may need to apply `edgesIgnoringSafeArea(_:)` to the container instead.

## See Also

### Deprecated Layout Modifiers

func frame() -> some View

Positions this view within an invisible frame.

Deprecated

func overlay&lt;Overlay>(Overlay, alignment: Alignment) -> some View

Layers a secondary view in front of this view.

func background&lt;Background>(Background, alignment: Alignment) -> some View

Layers the given view behind this view.

