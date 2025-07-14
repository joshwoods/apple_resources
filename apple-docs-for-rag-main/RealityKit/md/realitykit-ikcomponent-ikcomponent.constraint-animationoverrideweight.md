

- RealityKit
- IKComponent
- IKComponent.Constraint
-  animationOverrideWeight 

Instance Property

# animationOverrideWeight

The blending weights between the FK demand and the your target per demand type.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var animationOverrideWeight: (position: Float, rotation: Float) { get set }
```

## Discussion

Each demand uses either the value you set using target and lookAtTargetPosition, or computes one from the FK demand pose. These weights control the blending between the two.

The values are in the closed range `[0, 1]`, where a weight value of `0` means the constraint demands are computed from the FK demand, and a weight value of `1` means that target is used. All values in-between represent linear blend of the two. Default values are 0.

