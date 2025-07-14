

- GameplayKit
- GKPath
-  init(graphNodes:radius:) 

Initializer

# init(graphNodes:radius:)

Initializes a path using the positions of the specified graph nodes.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
init(
    graphNodes: [GKGraphNode],
    radius: Float
)
```

## Parameters 

`graphNodes`  

An array of graph node objects containing 2D points.

`radius`  

The radius of the path.

## Return Value

A new path object.

## Discussion

Use this initializer to turn a list of nodes from a navigation graph (as returned by the GKGraph findPath(from:to:) method) into a path-following goal for an agent. If the nodes are GKGraphNode2D objects, this initializer creates a 2D path; if the nodes are GKGraphNode3D objects, this initializer creates a 3D path.

The `radius` parameter defines the space occupied by the path—think of this space as the area created by sweeping a circle (or sphere, for 3D paths) of the specified radius along the path from vertex to vertex. Agents with path-related goals will attempt to move to or stay within this area.

To use the newly created path to constrain an agent’s behavior, create a goal with the init(toStayOn:maxPredictionTime:) or init(toFollow:maxPredictionTime:forward:) method.

