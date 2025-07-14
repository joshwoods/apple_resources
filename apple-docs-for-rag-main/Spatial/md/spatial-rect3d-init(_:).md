

- Spatial
- Rect3D
-  init(\_:) 

Initializer

# init(\_:)

Creates a rectangle structure from a bounding box.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+visionOS 1.0+

``` source
init(_ bounds: BoundingBox)
```

## See Also

### Creating a 3D rectangle structure

init()

Creates a rectangle structure.

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

Creates a rectangle at the specified origin and the specified size from Spatial structures.

init(origin: Point3D, size: Size3D)

Creates a rectangle structure.

init(points: [Point3D])

Creates a rectangle that’s the bounding box of the specified points.

