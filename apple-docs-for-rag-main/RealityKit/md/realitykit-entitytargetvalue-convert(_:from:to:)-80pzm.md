

- RealityKit
- EntityTargetValue
-  convert(\_:from:to:) 

Instance Method

# convert(\_:from:to:)

ConvConverts a 3D vector from a SwiftUI coordinate space to one in a RealityKit coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    _ vector: Vector3D,
    from space: some CoordinateSpaceProtocol,
    to realitySpace: some RealityCoordinateSpace
) -> SIMD3
```

