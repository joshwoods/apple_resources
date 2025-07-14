

- RealityKit
- RealityCoordinateSpaceConverting
-  convert(vector:from:to:) 

Instance Method

# convert(vector:from:to:)

Converts a 3D vector from a RealityKit coordinate space to one in a SwiftUI coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    vector: SIMD3,
    from realitySpace: some RealityCoordinateSpace,
    to space: some CoordinateSpaceProtocol
) -> Vector3D
```

