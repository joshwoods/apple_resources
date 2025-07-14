

- GameplayKit
- GKOctree
-  remove(\_:) 

Instance Method

# remove(\_:)

Searches for the specified object and removes it from the tree.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func remove(_ element: ElementType) -> Bool
```

## Parameters 

`element`  

The object to be removed from the tree.

## Return Value

true if the object was removed from the tree. false if the specified object is not in the tree.

## Discussion

The tree does not directly reference its elements—octrees are optimized to search for elements based on spatial positions—so this method must exhaustively search the entire tree to find the object to remove. For quicker removal, keep a reference to the GKOctreeNode object returned when you add an object to the tree, and call the remove(_:using:) method instead.

## See Also

### Adding and Removing Elements

func add(ElementType, at: vector_float3) -> GKOctreeNode

Adds an object to the tree corresponding to the specified point in 3D space.

func add(ElementType, in: GKBox) -> GKOctreeNode

Adds an object to the tree corresponding to the specified volume of 3D space.

func remove(ElementType, using: GKOctreeNode) -> Bool

Removes the specified object from the tree, using a reference to its containing node.

