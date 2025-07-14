

- RealityKit
- Transform
-  init(scale:rotation:translation:) 

Initializer

# init(scale:rotation:translation:)

Creates a new transformation using the given values.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
init(
    scale: SIMD3 = SIMD3(x: 1, y: 1, z: 1),
    rotation: simd_quatf = simd_quaternion(0, 0, 0, 1),
    translation: SIMD3 = SIMD3(x: 0, y: 0, z: 0)
)
```

## Parameters 

`scale`  

A scale factor.

`rotation`  

The rotation given as a unit quaternion.

`translation`  

The translation, or position along the x, y, and z axes.

## See Also

### Creating a transform

init()

Creates a transform with the values of the identity transform.

init(pitch: Float, yaw: Float, roll: Float)

Creates a new transform from the specified Euler angles.

init(matrix: float4x4)

Creates a new transform represented as a 4x4 matrix.

