

- RealityKit
- EntityTargetValue
-  unproject(\_:to:) 

Instance Method

# unproject(\_:to:)

Unproject a 2D point from the gesture value into 3D world coordinates.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
func unproject(
    _ keyPath: KeyPath,
    to realitySpace: some RealityCoordinateSpace
) -> SIMD3?
```

## Parameters 

`keyPath`  

A key path for a point on the gesture value.

`realitySpace`  

The 3D coordinate space of the returned point.

## Return Value

3D position in `realitySpace`.

