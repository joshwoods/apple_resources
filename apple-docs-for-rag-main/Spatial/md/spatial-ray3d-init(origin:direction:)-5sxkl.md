

- Spatial
- Ray3D
-  init(origin:direction:) 

Initializer

# init(origin:direction:)

Creates a ray with the specified origin and the specified direction from Spatial primitives.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    origin: Point3D,
    direction: Vector3D
)
```

## Parameters 

`origin`  

A point that specifies the ray’s origin.

`direction`  

A vector that specifies the ray’s direction.

## See Also

### Creating a 3D ray structure

init()

Creates a ray structure.

init(origin: simd_float3, direction: simd_float3)

Creates a ray with the specified origin and the specified direction from single-precision vectors.

init(origin: simd_double3, direction: simd_double3)

Creates a ray with the specified origin and the specified direction from double-precision vectors.

