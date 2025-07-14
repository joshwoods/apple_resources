

- RealityKit
- RealityViewContent
-  convert(size:from:to:) 

Instance Method

# convert(size:from:to:)

Converts a 3D size vector from a RealityKit coordinate space to a Size3D in a defined SwiftUI coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    size: SIMD3,
    from realitySpace: some RealityCoordinateSpace,
    to space: some CoordinateSpaceProtocol
) -> Size3D
```

