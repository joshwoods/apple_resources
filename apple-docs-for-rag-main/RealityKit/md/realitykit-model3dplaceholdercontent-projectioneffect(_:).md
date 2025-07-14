

- RealityKit
- Model3DPlaceholderContent
-  projectionEffect(\_:) 

Instance Method

# projectionEffect(\_:)

Applies a projection transformation to this view’s rendered output.

RealityKitSwiftUIiOS 13.0+iPadOS 13.0+macOS 10.15+tvOS 13.0+visionOSwatchOS 6.0+

``` source
nonisolated
func projectionEffect(_ transform: ProjectionTransform) -> some View
```

## Parameters 

`transform`  

A `ProjectionTransform` to apply to the view.

## Discussion

Use `projectionEffect(_:)` to apply a 3D transformation to the view.

The example below rotates the text 30˚ around the `z` axis, which is the axis pointing out of the screen:

```
// This transform represents a 30˚ rotation around the z axis.
let transform = CATransform3DMakeRotation(
    -30 * (.pi / 180), 0.0, 0.0, 1.0)

Text("Projection effects using transforms")
    .projectionEffect(.init(transform))
    .border(Color.gray)
```

