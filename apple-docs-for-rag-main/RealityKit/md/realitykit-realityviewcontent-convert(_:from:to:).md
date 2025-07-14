

- RealityKit
- RealityViewContent
-  convert(\_:from:to:) 

Instance Method

# convert(\_:from:to:)

Converts a Rect3D from a defined SwiftUI coordinate space to a BoundingBox in a RealityKit coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    _ rect: Rect3D,
    from space: some CoordinateSpaceProtocol,
    to realitySpace: some RealityCoordinateSpace
) -> BoundingBox
```

