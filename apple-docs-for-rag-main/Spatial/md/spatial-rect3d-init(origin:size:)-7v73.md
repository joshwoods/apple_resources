

- Spatial
- Rect3D
-  init(origin:size:) 

Initializer

# init(origin:size:)

Creates a rectangle at the specified origin and the specified size from Spatial structures.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 9.0+

``` source
init(
    origin: Point3D,
    size: Size3D
)
```

## Parameters 

`origin`  

A point structure that specifies the rectangle’s origin.

`size`  

A size structure that specifies the rectangle’s size.

## See Also

### Creating a 3D rectangle structure

init()

Creates a rectangle structure.

init(BoundingBox)

Creates a rectangle structure from a bounding box.

init(center: Point3D, size: Size3D)

Creates a rectangle with the specified center and the specified size from Spatial structures.

init(center: simd_double3, size: simd_double3)

Creates a rectangle with the specified center and the specified size from double-precision vectors.

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

Creates a rectangle structure.

init(points: [Point3D])

Creates a rectangle that’s the bounding box of the specified points.

