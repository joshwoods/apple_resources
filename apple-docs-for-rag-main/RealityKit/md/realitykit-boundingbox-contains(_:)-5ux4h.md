

- RealityKit
- BoundingBox
-  contains(\_:) 

Instance Method

# contains(\_:)

Checks whether the bounding box contains the specified bounds.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
func contains(_ boundingBox: BoundingBox) -> Bool
```

## Return Value

A Boolean that’s `true` if the box contains the specified bounds.

## See Also

### Checking for overlap

func contains(SIMD3&lt;Float>) -> Bool

Checks whether the bounding box contains the specified point.

func intersects(BoundingBox) -> Bool

Checks whether the bounding box intersects the specified bounds.

