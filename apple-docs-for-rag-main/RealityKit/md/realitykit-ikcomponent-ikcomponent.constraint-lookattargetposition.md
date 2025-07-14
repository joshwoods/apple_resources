

- RealityKit
- IKComponent
- IKComponent.Constraint
-  lookAtTargetPosition 

Instance Property

# lookAtTargetPosition

The point demand which the look-at constraint uses to generate a new orientation demand.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var lookAtTargetPosition: SIMD3 { get set }
```

## Discussion

The position is in model space. The computed demand overrides the rotation part of target.

