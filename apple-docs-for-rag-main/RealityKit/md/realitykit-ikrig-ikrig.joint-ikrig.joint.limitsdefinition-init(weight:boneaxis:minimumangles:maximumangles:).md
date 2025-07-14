

- RealityKit
- IKRig
- IKRig.Joint
- IKRig.Joint.LimitsDefinition
-  init(weight:boneAxis:minimumAngles:maximumAngles:) 

Initializer

# init(weight:boneAxis:minimumAngles:maximumAngles:)

Creates a joint limits definition.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 2.0+

``` source
init(
    weight: Float = 1.0,
    boneAxis: IKRig.Joint.LimitsDefinition.Axis = .x,
    minimumAngles: SIMD3 = [-2.0 * .pi, -2.0 * .pi, -2.0 * .pi],
    maximumAngles: SIMD3 = [2.0 * .pi, 2.0 * .pi, 2.0 * .pi]
)
```

## Parameters 

`weight`  

The weight of the joint rotation limit demand.

`boneAxis`  

The axis around which the bone twists.

`minimumAngles`  

The negative delta from the rest pose per-axis in radians.

`maximumAngles`  

The positive delta from the rest pose per-axis in radians.

## Discussion

Important

The minimum angles need to be less than the maximum angles.

