

- SwiftUI
- View
-  position(x:y:) 

Instance Method

# position(x:y:)

Positions the center of this view at the specified coordinates in its parent’s coordinate space.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
nonisolated
func position(
    x: CGFloat = 0,
    y: CGFloat = 0
) -> some View
```

## Parameters 

`x`  

The x-coordinate at which to place the center of this view.

`y`  

The y-coordinate at which to place the center of this view.

## Return Value

A view that fixes the center of this view at `x` and `y`.

## Mentioned in 

Making fine adjustments to a view’s position

Building layouts with stack views

## Discussion

Use the `position(x:y:)` modifier to place the center of a view at a specific coordinate in the parent view using an `x` and `y` offset.

```
Text("Position by passing the x and y coordinates")
    .position(x: 175, y: 100)
    .border(Color.gray)
```

## See Also

### Adjusting a view’s position

Making fine adjustments to a view’s position

Shift the position of a view by applying the offset or position modifier.

func position(CGPoint) -> some View

Positions the center of this view at the specified point in its parent’s coordinate space.

func offset(CGSize) -> some View

Offset this view by the horizontal and vertical amount specified in the offset parameter.

func offset(x: CGFloat, y: CGFloat) -> some View

Offset this view by the specified horizontal and vertical distances.

func offset(z: CGFloat) -> some View

Brings a view forward in Z by the provided distance in points.

