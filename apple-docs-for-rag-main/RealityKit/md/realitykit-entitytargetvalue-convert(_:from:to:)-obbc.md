

- RealityKit
- EntityTargetValue
-  convert(\_:from:to:) 

Instance Method

# convert(\_:from:to:)

Converts a Size3D from a defined SwiftUI coordinate space to a 3D size vector in a RealityKit coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    _ size: Size3D,
    from space: some CoordinateSpaceProtocol,
    to realitySpace: some RealityCoordinateSpace
) -> SIMD3
```

