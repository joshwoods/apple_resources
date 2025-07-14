

- GameplayKit
- GKRTree
-  elements(inBoundingRectMin:rectMax:) 

Instance Method

# elements(inBoundingRectMin:rectMax:)

Searches the tree and returns all elements found within the specified bounding region.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+macOS 10.12+tvOS 10.0+visionOS 1.0+

``` source
func elements(
    inBoundingRectMin rectMin: vector_float2,
    rectMax: vector_float2
) -> [ElementType]
```

## Parameters 

`rectMin`  

The corner (with the lowest x- and y-coordinate values) of the bounding region to search.

`rectMax`  

The corner (with the highest x- and y-coordinate values) of the bounding region to search.

## Return Value

An array of objects stored in the tree whose bounding regions overlap the specified region. The array is empty if no such objects are found.

## See Also

### Searching for Elements

var queryReserve: Int

The number of elements to reserve space for when searching.

