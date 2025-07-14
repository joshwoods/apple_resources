

- TabularData
- ColumnSlice
-  underestimatedCount 

Instance Property

# underestimatedCount

A value less than or equal to the number of elements in the collection.

TabularDataSwiftiOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var underestimatedCount: Int { get }
```

## Discussion

Complexity

O(1) if the collection conforms to `RandomAccessCollection`; otherwise, O(*n*), where *n* is the length of the collection.

## See Also

### Inspecting a Column

var isEmpty: Bool

A Boolean value indicating whether the collection is empty.

var count: Int

The number of elements in the collection.

func makeIterator() -> IndexingIterator&lt;Self>

Returns an iterator over the elements of the collection.

