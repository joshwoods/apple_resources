

- GameplayKit
- GKOctree
-  init(boundingBox:minimumCellSize:) 

Initializer

# init(boundingBox:minimumCellSize:)

Initializes an octree with the specified dimensions.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
init(
    boundingBox box: GKBox,
    minimumCellSize minCellSize: Float
)
```

## Parameters 

`box`  

The axis-aligned rectangular bounding volume encompassing all possible elements of the tree. Elements added to the tree must lie entirely within this box.

`minCellSize`  

The minimum dimension (width, height, and depth) of a node in the tree.

## Return Value

A new octree object.

## Discussion

The `minCellSize` parameter controls the memory usage and performance of the tree. A lower value causes the tree to make more spatial divisions when adding elements; a higher value causes the tree to create fewer such divisions, but store more elements in each node. Which direction leads to better performance depends on the number and spatial arrangement of the elements you add to the tree—for best results, profile with different values to find one best suited to your app or game.

For more information, see GameplayKit Programming Guide.

