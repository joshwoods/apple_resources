

- Spatial
- Size3D
-  init(width:height:depth:) 

Initializer

# init(width:height:depth:)

Creates a size structure from the specified floating-point values.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    width: T,
    height: T,
    depth: T
) where T : BinaryFloatingPoint
```

## Parameters 

`width`  

A floating-point value that specifies the width.

`height`  

A floating-point value that specifies the height.

`depth`  

A floating-point value that specifies the depth.

## See Also

### Creating a 3D size structure

init()

Creates a size structure.

init(width: Double, height: Double, depth: Double)

Creates a size structure from the specified double-precision values.

init(simd_float3)

Creates a size structure from the specified single-precision vector.

init(simd_double3)

Creates a size structure from the specified double-precision vector.

init(vector: simd_double3)

Creates a size structure from the specified double-precision vector.

init(Point3D)

Creates a size structure from the specified Spatial point.

init(Vector3D)

Creates a size structure from the specified Spatial vector.

