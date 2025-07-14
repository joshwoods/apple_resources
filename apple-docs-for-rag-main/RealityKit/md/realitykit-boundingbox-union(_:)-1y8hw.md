

- RealityKit
- BoundingBox
-  union(\_:) 

Instance Method

# union(\_:)

Creates a bounding box containing the current bounds and the specified bounds.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
func union(_ other: BoundingBox) -> BoundingBox
```

## Parameters 

`other`  

Another bounding box.

## Return Value

The new bounding box.

## See Also

### Expanding boxes

func formUnion(BoundingBox)

Expands the bounding box to contain the specified bounds.

func union(SIMD3&lt;Float>) -> BoundingBox

Creates a bounding box containing the current bounds and the specified point.

func formUnion(SIMD3&lt;Float>)

Expands the bounding box to contain the specified point.

