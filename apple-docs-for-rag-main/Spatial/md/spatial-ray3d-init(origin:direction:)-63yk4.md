

- Spatial
- Ray3D
-  init(origin:direction:) 

Initializer

# init(origin:direction:)

Creates a ray from Spatial primitives that describe the origin and direction.

iOS 16.0+iPadOS 16.0+Mac CatalystmacOS 13.0+tvOS 16.0+visionOSwatchOS 9.0+

``` source
init(
    origin: Point3D = .zero,
    direction: Vector3D
)
```

## Parameters 

`origin`  

The origin of the ray.

`direction`  

The direction of the ray.

## Discussion

Note

This function normalizes the direction vector.

