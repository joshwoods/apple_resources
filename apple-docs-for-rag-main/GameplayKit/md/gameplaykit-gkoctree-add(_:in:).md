

- GameplayKit
- GKOctree
-  add(\_:in:) 

Instance Method

# add(\_:in:)

Adds an object to the tree corresponding to the specified volume of 3D space.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func add(
    _ element: ElementType,
    in box: GKBox
) -> GKOctreeNode
```

## Parameters 

`element`  

The object to add to the tree.

## Return Value

The tree node containing the newly added object.

## Discussion

The GKOctree class automatically creates nodes to manage the objects you add to the tree. If you expect to remove an element you’ve added, keep a reference to the node this method returns so you can use the remove(_:using:) method to remove that object quickly.

## See Also

### Adding and Removing Elements

func add(ElementType, at: vector_float3) -> GKOctreeNode

Adds an object to the tree corresponding to the specified point in 3D space.

func remove(ElementType, using: GKOctreeNode) -> Bool

Removes the specified object from the tree, using a reference to its containing node.

func remove(ElementType) -> Bool

Searches for the specified object and removes it from the tree.

