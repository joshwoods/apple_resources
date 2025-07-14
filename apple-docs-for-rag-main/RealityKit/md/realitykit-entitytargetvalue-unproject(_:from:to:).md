

- RealityKit
- EntityTargetValue
-  unproject(\_:from:to:) 

Instance Method

# unproject(\_:from:to:)

Unproject `point` from a 2D coordinate space into 3D world coordinates.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
func unproject(
    _ point: CGPoint,
    from space: some CoordinateSpaceProtocol,
    to realitySpace: some RealityCoordinateSpace
) -> SIMD3?
```

## Parameters 

`point`  

A point in the provided coordinate space.

`space`  

The 2D coordinate space in which to interpret the `point`.

`realitySpace`  

The 3D coordinate space of the returned point.

## Return Value

3D position in `realitySpace`.

