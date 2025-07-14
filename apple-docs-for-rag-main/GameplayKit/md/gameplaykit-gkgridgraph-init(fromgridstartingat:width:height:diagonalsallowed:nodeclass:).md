

- GameplayKit
- GKGridGraph
-  init(fromGridStartingAt:width:height:diagonalsAllowed:nodeClass:) 

Initializer

# init(fromGridStartingAt:width:height:diagonalsAllowed:nodeClass:)

Initializes a graph that describes an integer grid with the specified dimensions, using the specified node class.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    fromGridStartingAt position: vector_int2,
    width: Int32,
    height: Int32,
    diagonalsAllowed: Bool,
    nodeClass: AnyClass
)
```

## Parameters 

`position`  

The lowest x- and y-coordinates to appear in the grid.

`width`  

The number of possible x-coordinates in the grid.

`height`  

The number of possible y-coordinates in the grid.

`diagonalsAllowed`  

true to connect nodes in the grid to their diagonal neighbors; false to connect nodes only to their horizontal and vertical neighbors.

`nodeClass`  

The GKGridGraphNode subclass to use for nodes in the graph.

## Return Value

A new grid graph.

## Discussion

Use the `nodeClass` parameter to create a graph using a custom subclass of GKGridGraphNode. For example, your custom node class might override the cost(to:) method so that some nodes are more costly than others to travel through. Pathfinding in such a graph would favor indirect routes when a direct route has a higher cost.

All connections created through this method are bidirectional.

For more information, see GameplayKit Programming Guide.

## See Also

### Creating a Graph

init(fromGridStartingAt: vector_int2, width: Int32, height: Int32, diagonalsAllowed: Bool)

Initializes a graph that describes an integer grid with the specified dimensions.

