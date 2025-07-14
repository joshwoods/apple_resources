

- GameplayKit
- GKGridGraph
-  init(fromGridStartingAt:width:height:diagonalsAllowed:) 

Initializer

# init(fromGridStartingAt:width:height:diagonalsAllowed:)

Initializes a graph that describes an integer grid with the specified dimensions.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    fromGridStartingAt position: vector_int2,
    width: Int32,
    height: Int32,
    diagonalsAllowed: Bool
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

## Return Value

A new grid graph.

## Discussion

All connections created through this method are bidirectional.

## See Also

### Creating a Graph

init(fromGridStartingAt: vector_int2, width: Int32, height: Int32, diagonalsAllowed: Bool, nodeClass: AnyClass)

Initializes a graph that describes an integer grid with the specified dimensions, using the specified node class.

