

- RealityKit
- RealityCoordinateSpaceProjecting
-  hitTest(point:in:query:mask:) 

Instance Method

# hitTest(point:in:query:mask:)

Searches the scene for entities at the specified point in the view.

RealityKitSwiftUIiOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+macOS 15.0+

``` source
func hitTest(
    point: CGPoint,
    in space: some CoordinateSpaceProtocol,
    query: CollisionCastQueryType,
    mask: CollisionGroup
) -> [CollisionCastHit]
```

**Required**

## Parameters 

`point`  

A point in the provided coordinate space.

`space`  

The 2D coordinate space in which to interpret the `point`.

`query`  

The query type.

`mask`  

The collision mask that you can use to prevent hits with certain objects. The default value is all, which means the ray can hit all objects. See CollisionFilter for details.

## Return Value

An array of hit-test results.

## Discussion

Important

RealityKit performs hit tests (ray-casts) against collision shapes. Entities without a proper CollisionComponent are ignored by hit tests.

