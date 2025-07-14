

- Spatial
- Ray3D
-  init(origin:direction:) 

Initializer

# init(origin:direction:)

Creates a ray with the specified origin and the specified direction from single-precision vectors.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    origin: simd_float3 = .zero,
    direction: simd_float3
)
```

## Parameters 

`origin`  

A vector that specifies the ray’s origin.

`direction`  

A vector that specifies the ray’s direction.

## See Also

### Creating a 3D ray structure

init()

Creates a ray structure.

init(origin: Point3D, direction: Vector3D)

Creates a ray with the specified origin and the specified direction from Spatial primitives.

init(origin: simd_double3, direction: simd_double3)

Creates a ray with the specified origin and the specified direction from double-precision vectors.

