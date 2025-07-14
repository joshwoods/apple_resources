

- RealityKit
- RealityViewCameraContent
-  entities(at:in:) 

Instance Method

# entities(at:in:)

Finds all the hit entities when projecting a ray from a starting point.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
func entities(
    at point: CGPoint,
    in space: some CoordinateSpaceProtocol
) -> [Entity]
```

## Parameters 

`point`  

A point in the provided coordinate space.

`space`  

The 2D coordinate space in which to interpret the `point`.

## Return Value

A list of entities at `point`. Returns an empty array if no entities were found.

## Discussion

Important

RealityKit performs hit tests (ray-casts) against collision shapes. Entities without a valid CollisionComponent are ignored by hit tests.

