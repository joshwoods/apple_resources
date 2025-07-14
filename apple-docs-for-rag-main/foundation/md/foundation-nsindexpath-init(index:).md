

- Foundation
- NSIndexPath
-  init(index:) 

Initializer

# init(index:)

Initializes an index path with a single node.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
convenience init(index: Int)
```

## Parameters 

`index`  

Index of the item in node 0 to point to.

## Return Value

Initialized NSIndexPath object representing a one-node index path with `index`.

## See Also

### Creating and Initializing Index Paths

init(indexes: UnsafePointer&lt;Int>?, length: Int)

Initializes an index path with the given nodes and length.

