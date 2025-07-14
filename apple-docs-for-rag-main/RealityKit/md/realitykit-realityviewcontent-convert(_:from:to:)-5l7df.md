

- RealityKit
- RealityViewContent
-  convert(\_:from:to:) 

Instance Method

# convert(\_:from:to:)

Converts a Rotation3D from a defined SwiftUI coordinate space to a quaternion in a RealityKit coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    _ rotation: Rotation3D,
    from space: some CoordinateSpaceProtocol,
    to realitySpace: some RealityCoordinateSpace
) -> simd_quatf
```

## Discussion

This function performs a change-of-basis operation, so the returned quaternion performs the same transformation in `realitySpace` that the specified `Rotation3D` performs in `space`.

