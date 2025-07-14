

- GameplayKit
- GKGraphNode
-  findPath(to:) 

Instance Method

# findPath(to:)

Computes and returns a sequence of nodes that represents the lowest-cost graph traversal from this node to the specified node.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
func findPath(to goalNode: GKGraphNode) -> [GKGraphNode]
```

## Parameters 

`goalNode`  

The destination node to which to attempt traversal of the graph.

## Return Value

An array of nodes representing a path through the graph in start to end order, or an empty array if no path exists between the specified nodes.

## Discussion

The returned array contains the list of nodes one must traverse in order to follow the selected route, starting with the requested `startNode` object, proceeding along the connections between nodes, and ending with the requested `endNode` object. For graphs whose nodes contain geometry information (GKGraphNode2D or GKGridGraphNode objects), you can use the information from each node in the array to move a game object along the path (or otherwise present the path to the user). Or, to make an agent (a GKAgent object) automatically follow the returned path, create a GKPath object with the init(graphNodes:radius:) initializer.

Calling this method is equivalent to calling the GKGraph findPath(from:to:) method when both nodes are in the same graph. However, when you instead use the findPath(to:) method of a specific node, GameplayKit finds a path (if one exists) through connected nodes to the destination node regardless of whether both nodes are contained in the same GKGraph object. This approach can be useful for connecting graphs that should otherwise be distinct. For example, each major area of your game world might have its own GKGraph object. When the player is near enough to a new area to move into it, you can connect a node of that area’s graph to the current area’s graph. Then, after the player has left an area behind, you can disconnect its graph and unload related content to save memory.

## See Also

### Finding Paths

func findPath(from: GKGraphNode) -> [GKGraphNode]

Computes and returns a sequence of nodes that represents the lowest-cost graph traversal from the specified node to this node.

