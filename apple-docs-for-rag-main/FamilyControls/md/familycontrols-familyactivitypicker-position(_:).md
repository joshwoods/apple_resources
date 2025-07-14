

- FamilyControls
- FamilyActivityPicker
-  position(\_:) 

Instance Method

# position(\_:)

Positions the center of this view at the specified point in its parent’s coordinate space.

FamilyControlsSwiftUIiOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+tvOS 13.0+watchOS 6.0+

``` source
nonisolated
func position(_ position: CGPoint) -> some View
```

## Parameters 

`position`  

The point at which to place the center of this view.

## Return Value

A view that fixes the center of this view at `position`.

## Discussion

Use the `position(_:)` modifier to place the center of a view at a specific coordinate in the parent view using a CGPoint to specify the `x` and `y` offset.

```
Text("Position by passing a CGPoint()")
    .position(CGPoint(x: 175, y: 100))
    .border(Color.gray)
```

## See Also

### Position

func position(x: CGFloat, y: CGFloat) -> some View

Positions the center of this view at the specified coordinates in its parent’s coordinate space.

func offset(CGSize) -> some View

Offset this view by the horizontal and vertical amount specified in the offset parameter.

func offset(x: CGFloat, y: CGFloat) -> some View

Offset this view by the specified horizontal and vertical distances.

func coordinateSpace&lt;T>(name: T) -> some View

Assigns a name to the view’s coordinate space, so other code can operate on dimensions like points and sizes relative to the named space.

