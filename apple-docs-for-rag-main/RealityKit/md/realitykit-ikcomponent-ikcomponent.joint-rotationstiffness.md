

- RealityKit
- IKComponent
- IKComponent.Joint
-  rotationStiffness 

Instance Property

# rotationStiffness

The per-axis rotational stiffness of the joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var rotationStiffness: SIMD3 { get set }
```

## Discussion

A joint with higher stiffness will rotate less to reach demands.

This value is in the closed range `[0, 1]`, where `0` means the joint is free to rotate, and `1` allows no movement.

