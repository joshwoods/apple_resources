

- GameplayKit
- GKGridGraph
-  diagonalsAllowed 

Instance Property

# diagonalsAllowed

A Boolean value that indicates whether nodes in the grid are connected to their diagonal neighbors.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var diagonalsAllowed: Bool { get }
```

## Discussion

If this property’s value is true, nodes in the grid are connected to their diagonal neighbors. If the value is false, nodes are connected only to their horizontal and vertical neighbors.

You specify this option when creating a grid graph with the init(fromGridStartingAt:width:height:diagonalsAllowed:) initializer. After initialization, you can use this property to examine the parameters the graph was created with—for example, to draw the grid as a debugging overlay in your game UI.

## See Also

### Inspecting a Graph

var gridOrigin: vector_int2

The lowest x- and y-coordinates that appear in the grid.

var gridWidth: Int

The number of possible x-coordinates in the grid.

var gridHeight: Int

The number of possible y-coordinates in the grid.

