

- RealityKit
- RealityCoordinateSpaceConverting
-  convert(point:from:to:) 

Instance Method

# convert(point:from:to:)

Converts a 3D point from a RealityKit coordinate space to one in a SwiftUI coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    point: SIMD3,
    from realitySpace: some RealityCoordinateSpace,
    to space: some CoordinateSpaceProtocol
) -> Point3D
```

