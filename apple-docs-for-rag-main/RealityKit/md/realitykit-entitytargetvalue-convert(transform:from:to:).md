

- RealityKit
- EntityTargetValue
-  convert(transform:from:to:) 

Instance Method

# convert(transform:from:to:)

Returns an AffineTransform3D converted from a RealityKit coordinate space to a defined SwiftUI coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    transform: Transform,
    from realitySpace: some RealityCoordinateSpace,
    to space: some CoordinateSpaceProtocol
) -> AffineTransform3D
```

## Discussion

This function performs a change-of-basis operation, so the returned `AffineTransform3D` performs the same transformation in `space` that the specified Transform performs in `realitySpace`.

