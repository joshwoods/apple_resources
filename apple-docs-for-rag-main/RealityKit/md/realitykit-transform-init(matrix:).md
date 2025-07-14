

- RealityKit
- Transform
-  init(matrix:) 

Initializer

# init(matrix:)

Creates a new transform represented as a 4x4 matrix.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
init(matrix: float4x4)
```

## Parameters 

`matrix`  

A transformation matrix.

## Discussion

A Transform component can’t represent every transform that a general 4x4 matrix can . Using a 4x4 matrix during initialization might result in certain transformations, such as shear, being lost.

## See Also

### Creating a transform

init()

Creates a transform with the values of the identity transform.

init(scale: SIMD3&lt;Float>, rotation: simd_quatf, translation: SIMD3&lt;Float>)

Creates a new transformation using the given values.

init(pitch: Float, yaw: Float, roll: Float)

Creates a new transform from the specified Euler angles.

