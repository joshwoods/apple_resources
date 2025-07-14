

- RealityKit
- EntityTargetValue
-  convert(\_:from:to:) 

Instance Method

# convert(\_:from:to:)

Converts a `Point3D` from a defined SwiftUI coordinate space to a 3D point in a RealityKit coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    _ point: Point3D,
    from space: some CoordinateSpaceProtocol,
    to realitySpace: some RealityCoordinateSpace
) -> SIMD3
```

