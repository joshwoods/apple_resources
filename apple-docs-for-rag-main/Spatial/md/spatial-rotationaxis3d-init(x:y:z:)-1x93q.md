

- Spatial
- RotationAxis3D
-  init(x:y:z:) 

Initializer

# init(x:y:z:)

Creates a rotation axis from the specified floating-point values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    x: T,
    y: T,
    z: T
) where T : BinaryFloatingPoint
```

## Parameters 

`x`  

A floating-point value that specifies the x-coordinate value.

`y`  

A floating-point value that specifies the y-coordinate value.

`z`  

A floating-point value that specifies the z-coordinate value.

## See Also

### Creating a 3D rotation axis structure

init()

Creates a rotation axis.

init(simd_float3)

Creates a rotation axis from the specified single-precision vector.

init(simd_double3)

Creates a rotation axis from the specified double-precision vector.

init(vector: simd_double3)

Creates a rotation axis from a three-element double-precision vector.

init(Vector3D)

Creates a rotation axis from a Spatial vector.

init(x: Double, y: Double, z: Double)

Creates a rotation axis from the specified double-precision values.

