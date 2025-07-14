

- RealityKit
- Transform
-  init(pitch:yaw:roll:) 

Initializer

# init(pitch:yaw:roll:)

Creates a new transform from the specified Euler angles.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
init(
    pitch x: Float = 0,
    yaw y: Float = 0,
    roll z: Float = 0
)
```

## Parameters 

`x`  

The rotation around the x-axis in radians.

`y`  

The rotation around the y-axis in radians.

`z`  

The rotation around the z-axis in radians.

## Discussion

The rotation order using intrinsic rotation order is defined as:

1.  Rotate around y-axis (yaw). 2. Rotate around the body-fixed x-axis (pitch). 3. Rotate around the body-fixed z-axis (roll).

The rotation order using extrinsic rotation order is defined as:

1.  Rotate around the z-axis (roll). 2. Rotate around the world space x-axis (pitch). 3. Rotate around the world space y-axis (yaw).

## See Also

### Creating a transform

init()

Creates a transform with the values of the identity transform.

init(scale: SIMD3&lt;Float>, rotation: simd_quatf, translation: SIMD3&lt;Float>)

Creates a new transformation using the given values.

init(matrix: float4x4)

Creates a new transform represented as a 4x4 matrix.

