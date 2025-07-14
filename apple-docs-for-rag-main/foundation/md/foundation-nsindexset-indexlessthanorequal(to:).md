

- Foundation
- NSIndexSet
-  indexLessThanOrEqual(to:) 

Instance Method

# indexLessThanOrEqual(to:)

Returns either the closest index in the index set that is less than or equal to a specific index or the not-found indicator.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
func indexLessThanOrEqual(to value: Int) -> Int
```

## Parameters 

`value`  

Index being inquired about.

## Return Value

Closest index in the index set less than or equal to `index`; NSNotFound when the index set contains no qualifying index.

## See Also

### Getting Indexes

var firstIndex: Int

The first index in the index set.

var lastIndex: Int

The last index in the index set.

func indexLessThanIndex(Int) -> Int

Returns either the closest index in the index set that is less than a specific index or the not-found indicator.

func indexGreaterThanOrEqual(to: Int) -> Int

Returns either the closest index in the index set that is greater than or equal to a specific index or the not-found indicator.

func indexGreaterThanIndex(Int) -> Int

Returns either the closest index in the index set that is greater than a specific index or the not-found indicator.

func getIndexes(UnsafeMutablePointer&lt;Int>, maxCount: Int, inIndexRange: NSRangePointer?) -> Int

The index set fills an index buffer with the indexes contained both in the index set and in an index range, returning the number of indexes copied.

