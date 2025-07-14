

- RealityKit
- EntityTargetValue
-  convert(\_:from:to:) 

Instance Method

# convert(\_:from:to:)

Returns a 3D Transform converted from a defined SwiftUI coordinate space to a RealityKit coordinate space.

RealityKitSwiftUIvisionOS 1.0+

``` source
func convert(
    _ transform: AffineTransform3D,
    from space: some CoordinateSpaceProtocol,
    to realitySpace: some RealityCoordinateSpace
) -> Transform
```

## Discussion

This function performs a change-of-basis operation, so the returned Transform performs the same transformation in `realitySpace` that the specified `AffineTransform3D` performs in `space`.

