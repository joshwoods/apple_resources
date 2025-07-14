

- Spatial
- Vector3D
-  init(x:y:z:) 

Initializer

# init(x:y:z:)

Creates a vector from the specified floating-point values.

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

A floating-point value that specifies the x value.

`y`  

A floating-point value that specifies the y value.

`z`  

A floating-point value that specifies the z value.

## See Also

### Creating a vector

init()

Creates a vector.

init(x: Double, y: Double, z: Double)

Creates a vector from the specified double-precision values.

init(simd_float3)

Creates a ray from the specified single-precision vector.

init(simd_double3)

Creates a vector from the specified double-precision vector.

init(vector: simd_double3)

Creates a vector from the specified double-precision vector.

init(RotationAxis3D)

Creates a vector from the specified Spatial rotation axis.

init(Point3D)

Creates a vector from the specified Spatial point structure.

init(Size3D)

Creates a vector from the specified Spatial size structure.

init(SphericalCoordinates3D)

Creates a vector from the specified Spatial spherical coordinates structure.

