

- GameplayKit
- GKQuadtree
-  elements(in:) 

Instance Method

# elements(in:)

Returns all objects whose corresponding locations overlap the specified region.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func elements(in quad: GKQuad) -> [ElementType]
```

## Parameters 

`quad`  

The axis-aligned rectangle in 2D space to search.

## Return Value

An array of all matching elements, or an empty array if no objects are found.

## Discussion

You specify the point or region corresponding to an object when you add it to the tree with the add(_:at:) or add(_:in:) method. This method follows the same path down the tree as the two `addElement` methods, but instead of adding a new object to the tree, returns the list of all objects stored in the tree node corresponding to the specified point.

## See Also

### Searching for Elements

func elements(at: vector_float2) -> [ElementType]

Returns all objects whose corresponding locations overlap the specified point.

