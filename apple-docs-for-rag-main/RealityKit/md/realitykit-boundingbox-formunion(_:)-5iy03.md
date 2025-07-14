

- RealityKit
- BoundingBox
-  formUnion(\_:) 

Instance Method

# formUnion(\_:)

Expands the bounding box to contain the specified bounds.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
mutating func formUnion(_ other: BoundingBox)
```

## Parameters 

`other`  

Another bounding box.

## See Also

### Expanding boxes

func union(BoundingBox) -> BoundingBox

Creates a bounding box containing the current bounds and the specified bounds.

func union(SIMD3&lt;Float>) -> BoundingBox

Creates a bounding box containing the current bounds and the specified point.

func formUnion(SIMD3&lt;Float>)

Expands the bounding box to contain the specified point.

