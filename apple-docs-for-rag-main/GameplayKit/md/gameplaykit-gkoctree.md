

- GameplayKit
-  GKOctree 

Class

# GKOctree

A data structure for organizing objects based on their locations in a three-dimensional space.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class GKOctree where ElementType : NSObject
```

## Overview

An octree manages its structure to optimize for spatial searches—unlike a basic data structure such as an array or dictionary, an octree can find all elements occupying a specific position or volume very quickly. The octree partitioning strategy divides space into eight octants at each level, as illustrated in Figure 1. When an octant contains more than one object, the tree subdivides that region into eight smaller octants, adding a level to the tree.

Octrees can be useful for many tasks in game design. For example:

- Deciding which game characters are close enough to each other for interaction

- Deciding which portions of a large game world need to be processed at a given time

The GKOctree class is one of three spatial partitioning data structures that GameplayKit provides, and the only one suited to three-dimensional data. See the `GKQuadTree` class for the two-dimensional analogue of an octree, and the GKRTree class for different ways to organize two-dimensional data.

## Topics

### Creating an Octree

init(boundingBox: GKBox, minimumCellSize: Float)

Initializes an octree with the specified dimensions.

### Adding and Removing Elements

func add(ElementType, at: vector_float3) -> GKOctreeNode

Adds an object to the tree corresponding to the specified point in 3D space.

func add(ElementType, in: GKBox) -> GKOctreeNode

Adds an object to the tree corresponding to the specified volume of 3D space.

func remove(ElementType, using: GKOctreeNode) -> Bool

Removes the specified object from the tree, using a reference to its containing node.

func remove(ElementType) -> Bool

Searches for the specified object and removes it from the tree.

### Searching for Elements

func elements(at: vector_float3) -> [ElementType]

Returns all objects whose corresponding locations overlap the specified point.

func elements(in: GKBox) -> [ElementType]

Returns all objects whose corresponding locations overlap the specified volume.

### Constants

struct GKBox

The definition of an axis-aligned rectangular bounding volume addressed by the tree.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Spatial Partitioning

class GKQuadtree

A data structure for organizing objects based on their locations in a two-dimensional space.

class GKQuadtreeNode

A helper class for managing the objects you organize in a quadtree.

class GKOctreeNode

A helper class for managing the objects you organize in an octree.

class GKRTree

A data structure that adaptively organizes objects based on their locations in a two-dimensional space.

