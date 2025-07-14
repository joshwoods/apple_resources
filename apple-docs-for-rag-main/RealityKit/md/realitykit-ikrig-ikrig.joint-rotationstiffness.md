

- RealityKit
- IKRig
- IKRig.Joint
-  rotationStiffness 

Instance Property

# rotationStiffness

The per-axis rotational stiffness of the joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var rotationStiffness: SIMD3
```

## Discussion

A joint with higher stiffness rotates less to reach demands.

Values are in the closed range `[0, 1]`, where `0` means free to rotate, and `1` is no movement.

