

- SwiftUI
- View
-  fixedSize(horizontal:vertical:) 

Instance Method

# fixedSize(horizontal:vertical:)

Fixes this view at its ideal size in the specified dimensions.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func fixedSize(
    horizontal: Bool,
    vertical: Bool
) -> some View
```

## Parameters 

`horizontal`  

A Boolean value that indicates whether to fix the width of the view.

`vertical`  

A Boolean value that indicates whether to fix the height of the view.

## Return Value

A view that fixes this view at its ideal size in the dimensions specified by `horizontal` and `vertical`.

## Discussion

This function behaves like fixedSize(), except with `fixedSize(horizontal:vertical:)` the fixing of the axes can be optionally specified in one or both dimensions. For example, if you horizontally fix a text view before wrapping it in the frame view, you’re telling the text view to maintain its ideal *width*. The view calculates this to be the space needed to represent the entire string.

```
Text("A single line of text, too long to fit in a box.")
    .fixedSize(horizontal: true, vertical: false)
    .frame(width: 200, height: 200)
    .border(Color.gray)
```

This can result in the view exceeding the parent’s bounds, which may or may not be the effect you want.

## See Also

### Influencing a view’s size

func frame(width: CGFloat?, height: CGFloat?, alignment: Alignment) -> some View

Positions this view within an invisible frame with the specified size.

func frame(depth: CGFloat?, alignment: DepthAlignment) -> some View

Positions this view within an invisible frame with the specified depth.

func frame(minWidth: CGFloat?, idealWidth: CGFloat?, maxWidth: CGFloat?, minHeight: CGFloat?, idealHeight: CGFloat?, maxHeight: CGFloat?, alignment: Alignment) -> some View

Positions this view within an invisible frame having the specified size constraints.

func frame(minDepth: CGFloat?, idealDepth: CGFloat?, maxDepth: CGFloat?, alignment: DepthAlignment) -> some View

Positions this view within an invisible frame having the specified depth constraints.

func containerRelativeFrame(Axis.Set, alignment: Alignment) -> some View

Positions this view within an invisible frame with a size relative to the nearest container.

func containerRelativeFrame(Axis.Set, alignment: Alignment, (CGFloat, Axis) -> CGFloat) -> some View

Positions this view within an invisible frame with a size relative to the nearest container.

func containerRelativeFrame(Axis.Set, count: Int, span: Int, spacing: CGFloat, alignment: Alignment) -> some View

Positions this view within an invisible frame with a size relative to the nearest container.

func fixedSize() -> some View

Fixes this view at its ideal size.

func layoutPriority(Double) -> some View

Sets the priority by which a parent layout should apportion space to this child.

