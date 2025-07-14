

- RealityKit
- MeshResource
-  init(extruding:extrusionOptions:) 

Initializer

# init(extruding:extrusionOptions:)

Asynchronously generates a 3D mesh by extruding a 2D path.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+visionOS 2.0+

``` source
nonisolated
convenience init(
    extruding path: Path,
    extrusionOptions: MeshResource.ShapeExtrusionOptions = ShapeExtrusionOptions()
) async throws
```

## Parameters 

`path`  

A path that contains the starting shape for the 3D mesh geometry.

`extrusionOptions`  

A configuration for extruding the path in 3D.

## Discussion

The filled area of the path is determined using the even-odd winding rule (see Filling a Path in the Quartz 2D Programming Guide Guide). The provided path needs to satisfy the following conditions, or behavior is undefined:

1.  Subpaths contains no self intersections.

2.  Subpaths do not intersect each other.

3.  All subpaths are closed.

## See Also

### Creating a 3D mesh by extruding a 2D path

convenience init(extruding: Path, extrusionOptions: MeshResource.ShapeExtrusionOptions) throws

Synchronously generates a 3D mesh by extruding a 2D path.

