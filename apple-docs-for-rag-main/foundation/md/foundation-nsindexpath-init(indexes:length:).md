

- Foundation
- NSIndexPath
-  init(indexes:length:) 

Initializer

# init(indexes:length:)

Initializes an index path with the given nodes and length.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
init(
    indexes: UnsafePointer?,
    length: Int
)
```

## Parameters 

`indexes`  

Array of indexes to make up the index path.

`length`  

Number of nodes to include in the index path.

## Return Value

Initialized NSIndexPath object with `indexes` up to `length`.

## Discussion

This method is a designated initializer of NSIndexPath.

## See Also

### Creating and Initializing Index Paths

convenience init(index: Int)

Initializes an index path with a single node.

