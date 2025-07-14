

- RealityKit
- BoundingBox
-  contains(\_:) 

Instance Method

# contains(\_:)

Checks whether the bounding box contains the specified point.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
func contains(_ point: SIMD3) -> Bool
```

## Return Value

A Boolean that’s `true` if the box contains the specified point.

## See Also

### Checking for overlap

func contains(BoundingBox) -> Bool

Checks whether the bounding box contains the specified bounds.

func intersects(BoundingBox) -> Bool

Checks whether the bounding box intersects the specified bounds.

