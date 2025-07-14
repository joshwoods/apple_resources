

- Foundation
- NSIndexPath
-  adding(\_:) 

Instance Method

# adding(\_:)

Returns an index path containing the nodes in the receiving index path plus another given index.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func adding(_ index: Int) -> IndexPath
```

## Parameters 

`index`  

Index to append to the index path’s indexes.

## Return Value

A new index path containing the receiving index path’s indexes and `index`.

## See Also

### Adding and Removing Nodes

func removingLastIndex() -> IndexPath

Returns an index path with the nodes in the receiving index path, excluding the last one.

