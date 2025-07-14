

- Foundation
- NSIndexSet
-  lastIndex 

Instance Property

# lastIndex

The last index in the index set.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
var lastIndex: Int { get }
```

## Discussion

Last index in the index set or NSNotFound when the index set is empty.

## See Also

### Getting Indexes

var firstIndex: Int

The first index in the index set.

func indexLessThanIndex(Int) -> Int

Returns either the closest index in the index set that is less than a specific index or the not-found indicator.

func indexLessThanOrEqual(to: Int) -> Int

Returns either the closest index in the index set that is less than or equal to a specific index or the not-found indicator.

func indexGreaterThanOrEqual(to: Int) -> Int

Returns either the closest index in the index set that is greater than or equal to a specific index or the not-found indicator.

func indexGreaterThanIndex(Int) -> Int

Returns either the closest index in the index set that is greater than a specific index or the not-found indicator.

func getIndexes(UnsafeMutablePointer&lt;Int>, maxCount: Int, inIndexRange: NSRangePointer?) -> Int

The index set fills an index buffer with the indexes contained both in the index set and in an index range, returning the number of indexes copied.

