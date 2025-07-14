

- Foundation
- NSIndexPath
-  index(atPosition:) 

Instance Method

# index(atPosition:)

Provides the value at a particular node in the index path.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func index(atPosition position: Int) -> Int
```

## Parameters 

`position`  

Index value of the desired node. Node numbering starts at zero.

## Return Value

The index value at `node` or `NSNotFound` if the node is outside the range of the index path.

## See Also

### Working with Indexes

func getIndexes(UnsafeMutablePointer&lt;Int>, range: NSRange)

Copies the indexes stored in the index path from the positions specified by the position range into the specified indexes.

func getIndexes(UnsafeMutablePointer&lt;Int>)

Copies the objects contained in the index path into indexes.

Deprecated

