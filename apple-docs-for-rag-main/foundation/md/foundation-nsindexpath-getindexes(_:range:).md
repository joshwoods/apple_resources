

- Foundation
- NSIndexPath
-  getIndexes(\_:range:) 

Instance Method

# getIndexes(\_:range:)

Copies the indexes stored in the index path from the positions specified by the position range into the specified indexes.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.9+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func getIndexes(
    _ indexes: UnsafeMutablePointer,
    range positionRange: NSRange
)
```

## Parameters 

`indexes`  

Pointer to a C array of at least as many NSUInteger objects as specified by the length of `positionRange`. On return, the array holds the index path’s indexes.

`positionRange`  

A range of valid positions within the index path. If the location plus the length of `positionRange` is greater than the length of the index path, this method raises an rangeException.

## Discussion

You must allocate the memory for the C array.

## See Also

### Working with Indexes

func index(atPosition: Int) -> Int

Provides the value at a particular node in the index path.

func getIndexes(UnsafeMutablePointer&lt;Int>)

Copies the objects contained in the index path into indexes.

Deprecated

