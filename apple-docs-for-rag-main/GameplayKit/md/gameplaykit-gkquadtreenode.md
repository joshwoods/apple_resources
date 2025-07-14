

- GameplayKit
-  GKQuadtreeNode 

Class

# GKQuadtreeNode

A helper class for managing the objects you organize in a quadtree.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
class GKQuadtreeNode
```

## Overview

You don’t create instances of this class directly; instead, a GKQuadtree object provides you with a GKQuadtreeNode instance when you add an element to a tree. If you plan to remove elements from the tree, keep references to the corresponding nodes so you can use the remove(_:using:) method for better performance.

For more information, see GameplayKit Programming Guide.

## Topics

### Examining a Node

var quad: GKQuad

The axis-aligned bounding rectangle represented by the node.

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

class GKOctree

A data structure for organizing objects based on their locations in a three-dimensional space.

class GKOctreeNode

A helper class for managing the objects you organize in an octree.

class GKRTree

A data structure that adaptively organizes objects based on their locations in a two-dimensional space.

