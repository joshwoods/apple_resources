

- GameplayKit
- GKRTree
-  addElement(\_:boundingRectMin:boundingRectMax:splitStrategy:) 

Instance Method

# addElement(\_:boundingRectMin:boundingRectMax:splitStrategy:)

Adds the specified object to the tree.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func addElement(
    _ element: ElementType,
    boundingRectMin: vector_float2,
    boundingRectMax: vector_float2,
    splitStrategy: GKRTreeSplitStrategy
)
```

## Parameters 

`element`  

The object to be added to the tree.

`boundingRectMin`  

The corner (with the lowest x- and y-coordinate values) of the bounding region occupied by the object.

`boundingRectMax`  

The corner (with the highest x- and y-coordinate values) of the bounding region occupied by the object.

`splitStrategy`  

An option specifying the algorithm the tree should use to optimize its internal structure after adding the new element.

## Discussion

The bounding region of each object you add to the tree (specified with the `boundingRectMin` and `boundingRectMax` parameters) defines the location and size of that object in space. When you add an object, depending on the relation of that size and position to those of other objects in the tree, the tree may reorganize its internal structure so that later searches of the tree (with the elements(inBoundingRectMin:rectMax:)) can perform more quickly.

The `splitStrategy` parameter controls how the tree reorganizes its internal structure when needed—you can use a different strategy each time you add an object. Which strategy provides the best performance depends on the organization of data in your app or game; for best results, experiment with different strategies and profile your app’s performance with each.

## See Also

### Adding and Removing Elements

func removeElement(ElementType, boundingRectMin: vector_float2, boundingRectMax: vector_float2)

Removes the specified object from the tree.

