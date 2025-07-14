

- GameplayKit
- GKGridGraphNode
-  gridPosition 

Instance Property

# gridPosition

The position of the node on a discrete integer grid.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var gridPosition: vector_int2 { get }
```

## Discussion

You specify the position only when creating a node.

When working with an array of nodes returned by the GKGraph findPath(from:to:) method, read the position from each node to determine the path for an entity in your game scene to follow.

