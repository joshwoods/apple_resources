

- GameplayKit
- GKQuadtree
-  add(\_:in:) 

Instance Method

# add(\_:in:)

Adds an object to the tree corresponding to the specified region of 2D space.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func add(
    _ element: ElementType,
    in quad: GKQuad
) -> GKQuadtreeNode
```

## Parameters 

`element`  

The object to add to the tree.

`quad`  

The axis-aligned bounding region in 2D space to which the object corresponds.

## Return Value

The tree node containing the newly added object.

## Discussion

The GKQuadtree class automatically creates nodes to manage the objects you add to the tree. If you expect to remove an element you’ve added, keep a reference to the node this method returns so you can use the remove(_:using:) method to remove that object quickly.

## See Also

### Adding and Removing Elements

func add(ElementType, at: vector_float2) -> GKQuadtreeNode

Adds an object to the tree corresponding to the specified point in 2D space.

func remove(ElementType, using: GKQuadtreeNode) -> Bool

Removes the specified object from the tree, using a reference to its containing node.

func remove(ElementType) -> Bool

Searches for the specified object and removes it from the tree.

