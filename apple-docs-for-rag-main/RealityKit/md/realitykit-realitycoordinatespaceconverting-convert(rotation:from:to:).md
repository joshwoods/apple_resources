

- RealityKit
- RealityCoordinateSpaceConverting
-  convert(rotation:from:to:) 

Instance Method

# convert(rotation:from:to:)

Converts a quaternion from a RealityKit coordinate space to a Rotation3D in a defined SwiftUI coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    rotation: simd_quatf,
    from realitySpace: some RealityCoordinateSpace,
    to space: some CoordinateSpaceProtocol
) -> Rotation3D
```

## Discussion

This function performs a change-of-basis operation, so the returned `Rotation3D` performs the same transformation in `space` that the specified quaternion performs in `realitySpace`.

