

- RealityKit
- BillboardComponent
-  blendFactor 

Instance Property

# blendFactor

The degree at which the entity rotates toward the camera.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var blendFactor: Float
```

## Discussion

The `blendFactor` property is a floating-point number in the range `[0.0, 1.0]`.

- When `blendFactor` is `1.0`, the entity fully faces the camera. This is the default behavior.

- When `blendFactor` is `0.0`, the entity doesn’t rotate at all.

- When `blendFactor` is between `0.0` and `1.0`, the entity partially rotates toward the camera.

The following example configures the entity to rotate by half the angle it needs to directly face the camera by setting the `blendFactor` to `0.5`:

```
var billboard = BillboardComponent()
billboard.blendFactor = 0.5
entity.components.set(billboard)
```

For example, here’s how a few different `blendFactor` values affect the orientation:

| 0 | 0.25 | 0.5 | 1 |
|----|----|----|----|
|  |  |  |  |

For an example of how to animate `blendFactor`, see BillboardAction.

