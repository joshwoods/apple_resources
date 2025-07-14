

- RealityKit
- RealityCoordinateSpaceProjecting
-  project(point:to:) 

Instance Method

# project(point:to:)

Projects a point from the 3D world coordinate system of the scene to the 2D pixel coordinate system of the reality view.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
func project(
    point: SIMD3,
    to space: some CoordinateSpaceProtocol
) -> CGPoint?
```

**Required**

## Parameters 

`point`  

The point in 3D world coordinates.

`space`  

The 2D coordinate space in which this function returns the point.

## Return Value

A point in the provided coordinate space.

