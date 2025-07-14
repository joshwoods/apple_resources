

- Spatial
- Rect3D
-  init(center:size:) 

Initializer

# init(center:size:)

Creates a rectangle with the specified center and the specified size from double-precision vectors.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    center: simd_double3 = .zero,
    size: simd_double3
)
```

## Parameters 

`center`  

A double-precision vector that specifies the rectangle’s center.

`size`  

A double-precision vector that specifies the rectangle’s size.

## See Also

### Creating a 3D rectangle structure

init()

Creates a rectangle structure.

init(BoundingBox)

Creates a rectangle structure from a bounding box.

init(center: Point3D, size: Size3D)

Creates a rectangle with the specified center and the specified size from Spatial structures.

init(center: Vector3D, size: Vector3D)

Creates a rectangle with the specified center and the specified size from Spatial vectors.

init(center: simd_float3, size: simd_float3)

Creates a rectangle with the specified center and the specified size from single-precision vectors.

init(origin: simd_double3, size: simd_double3)

Creates a rectangle at the specified origin with the specified size from double-precision vectors.

init(origin: simd_float3, size: simd_float3)

Creates a rectangle at the specified origin with the specified size from single-precision vectors.

init(origin: Vector3D, size: Vector3D)

Creates a rectangle with the specified origin and the specified size from Spatial vectors.

init(origin: Point3D, size: Size3D)

Creates a rectangle at the specified origin and the specified size from Spatial structures.

init(origin: Point3D, size: Size3D)

Creates a rectangle structure.

init(points: [Point3D])

Creates a rectangle that’s the bounding box of the specified points.

