

- RealityKit
- Model3DPlaceholderContent
-  position(\_:) 

Instance Method

# position(\_:)

Positions the center of this view at the specified point in its parent’s coordinate space.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

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

