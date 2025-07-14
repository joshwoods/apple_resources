

- GameplayKit
- GKQuadtree
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

The tree does not directly reference its elements—quadtrees are optimized to search for elements based on spatial positions—so this method must exhaustively search the entire tree to find the object to remove. For quicker removal, keep a reference to the GKQuadtreeNode object returned when you add an object to the tree, and call the remove(_:using:) method instead.

## See Also

### Adding and Removing Elements

func add(ElementType, at: vector_float2) -> GKQuadtreeNode

Adds an object to the tree corresponding to the specified point in 2D space.

func add(ElementType, in: GKQuad) -> GKQuadtreeNode

Adds an object to the tree corresponding to the specified region of 2D space.

func remove(ElementType, using: GKQuadtreeNode) -> Bool

Removes the specified object from the tree, using a reference to its containing node.

