

- RealityKit
- BoundingBox
-  union(\_:) 

Instance Method

# union(\_:)

Creates a bounding box containing the current bounds and the specified point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
func union(_ point: SIMD3) -> BoundingBox
```

## Parameters 

`point`  

A point in space.

## Return Value

The new bounding box.

## See Also

### Expanding boxes

func union(BoundingBox) -> BoundingBox

Creates a bounding box containing the current bounds and the specified bounds.

func formUnion(BoundingBox)

Expands the bounding box to contain the specified bounds.

func formUnion(SIMD3&lt;Float>)

Expands the bounding box to contain the specified point.

