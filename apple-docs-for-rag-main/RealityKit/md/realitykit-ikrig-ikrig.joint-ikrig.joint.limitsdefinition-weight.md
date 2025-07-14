

- RealityKit
- IKRig
- IKRig.Joint
- IKRig.Joint.LimitsDefinition
-  weight 

Instance Property

# weight

The weight of the joint rotation limit demand.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var weight: Float
```

## Discussion

The value is in the closed range `[0, 1]`, where `0` means no influence, and `1` is maximum correction.

