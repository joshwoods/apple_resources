

- RealityKit
- IKRig
-  globalLimitsWeight 

Instance Property

# globalLimitsWeight

The solver global weight for the joint rotation limits.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
var globalLimitsWeight: Float
```

## Discussion

This weight is a multiplier for each joint’s weight.

The recommended value range is the closed range `[0, 1]`, where `0` means no limits influence, and `1` is no rig level modification.

