

- SwiftUI
- View
-  offset(\_:) 

Instance Method

# offset(\_:)

Offset this view by the horizontal and vertical amount specified in the offset parameter.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func offset(_ offset: CGSize) -> some View
```

## Parameters 

`offset`  

The distance to offset this view.

## Return Value

A view that offsets this view by `offset`.

## Discussion

Use `offset(_:)` to shift the displayed contents by the amount specified in the `offset` parameter.

The original dimensions of the view aren’t changed by offsetting the contents; in the example below the gray border drawn by this view surrounds the original position of the text:

```
Text("Offset by passing CGSize()")
    .border(Color.green)
    .offset(CGSize(width: 20, height: 25))
    .border(Color.gray)
```

## See Also

### Adjusting a view’s position

Making fine adjustments to a view’s position

Shift the position of a view by applying the offset or position modifier.

func position(CGPoint) -> some View

Positions the center of this view at the specified point in its parent’s coordinate space.

func position(x: CGFloat, y: CGFloat) -> some View

Positions the center of this view at the specified coordinates in its parent’s coordinate space.

func offset(x: CGFloat, y: CGFloat) -> some View

Offset this view by the specified horizontal and vertical distances.

func offset(z: CGFloat) -> some View

Brings a view forward in Z by the provided distance in points.

