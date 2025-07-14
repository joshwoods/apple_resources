

- RealityKit
- IKComponent
- IKComponent.Joint
-  fkWeightPerAxis 

Instance Property

# fkWeightPerAxis

The per-axis weight of the source animation demand on the joint.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var fkWeightPerAxis: SIMD3 { get set }
```

## Discussion

This value is in the closed range `[0, 1]`, where `0` means no influence, and `1` is the maximum influence.

