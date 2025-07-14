

- RealityKit
- HasTransform
-  visualBounds(recursive:relativeTo:excludeInactive:) 

Instance Method

# visualBounds(recursive:relativeTo:excludeInactive:)

Computes a bounding box for the entity in the specified space, optionally including child entities.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.0+macOS 10.15+visionOS

``` source
@MainActor @preconcurrency
func visualBounds(
    recursive: Bool = true,
    relativeTo referenceEntity: Entity?,
    excludeInactive: Bool = false
) -> BoundingBox
```

## Parameters 

`recursive`  

A Boolean that you set to `true` to incorporate the bounds of all descendants.

`referenceEntity`  

An entity that defines a frame of reference. Set to `nil` to indicate world space.

`excludeInactive`  

A Boolean that you set to `true` to exclude inactive entities.

## Return Value

The bounding box.

## Discussion

The method has complexity `O(n)`, where `n` is the number of entities in the hierarchy.

