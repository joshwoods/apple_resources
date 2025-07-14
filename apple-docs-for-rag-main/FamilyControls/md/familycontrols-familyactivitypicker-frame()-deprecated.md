

- FamilyControls
- FamilyActivityPicker
-  frame() Deprecated

Instance Method

# frame()

Positions this view within an invisible frame.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func frame() -> some View
```

Deprecated

Please pass one or more parameters.

## Discussion

Use `SwiftUI/View/frame(width:height:alignment:)` or `SwiftUI/View/frame(minWidth:idealWidth:maxWidth:minHeight:idealHeight:maxHeight:alignment:)` instead.

## See Also

### Deprecated Layout Modifiers

func edgesIgnoringSafeArea(Edge.Set) -> some View

Changes the view’s proposed area to extend outside the screen’s safe areas.

func overlay&lt;Overlay>(Overlay, alignment: Alignment) -> some View

Layers a secondary view in front of this view.

func background&lt;Background>(Background, alignment: Alignment) -> some View

Layers the given view behind this view.

