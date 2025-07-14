

- GameplayKit
- GKQuadtree
-  remove(\_:using:) 

Instance Method

# remove(\_:using:)

Removes the specified object from the tree, using a reference to its containing node.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func remove(
    _ data: ElementType,
    using node: GKQuadtreeNode
) -> Bool
```

## Parameters 

`data`  

The object to be removed from the tree.

`node`  

The node in the tree containing the object.

## Return Value

true if the object was removed from the tree. false if the specified object or node is not in the tree.

## Discussion

By referencing the node that contains the object to remove, this method can quickly remove an object from the tree without needing to perform an exhaustive search. To make use of this performance optimization, keep a reference to the node returned when you add elements with the add(_:at:) or add(_:in:) methods.

## See Also

### Adding and Removing Elements

func add(ElementType, at: vector_float2) -> GKQuadtreeNode

Adds an object to the tree corresponding to the specified point in 2D space.

func add(ElementType, in: GKQuad) -> GKQuadtreeNode

Adds an object to the tree corresponding to the specified region of 2D space.

func remove(ElementType) -> Bool

Searches for the specified object and removes it from the tree.

