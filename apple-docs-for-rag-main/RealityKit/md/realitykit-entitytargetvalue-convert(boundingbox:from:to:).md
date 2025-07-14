

- RealityKit
- EntityTargetValue
-  convert(boundingBox:from:to:) 

Instance Method

# convert(boundingBox:from:to:)

Converts a BoundingBox from a RealityKit coordinate space to a Rect3D in a defined SwiftUI coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    boundingBox: BoundingBox,
    from realitySpace: some RealityCoordinateSpace,
    to space: some CoordinateSpaceProtocol
) -> Rect3D
```

