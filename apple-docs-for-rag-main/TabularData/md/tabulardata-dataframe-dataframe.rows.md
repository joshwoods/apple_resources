

- TabularData
- DataFrame
-  DataFrame.Rows 

Structure

# DataFrame.Rows

A collection of rows in a data frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Rows
```

## Topics

### Inspecting a Row Collection

var count: Int

The number of rows in the collection.

### Accessing Elements

subscript(Int) -> DataFrame.Row

Accesses a row at an index.

subscript(Range&lt;Int>) -> DataFrame.Rows

Returns a row collection from an index range.

### Type Aliases

typealias Element

A type representing the sequence’s elements.

typealias Index

A type that represents a position in the collection.

typealias Indices

A type that represents the indices that are valid for subscripting the collection, in ascending order.

typealias Iterator

A type that provides the collection’s iteration interface and encapsulates its iteration state.

typealias SubSequence

A collection representing a contiguous subrange of this collection’s elements. The subsequence shares indices with the original collection.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

MutableCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- MutableCollection
- Sequence

## See Also

### Inspecting a Data Frame

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number of rows and columns in the data frame.

var columns: [AnyColumn]

The entire data frame as a collection of columns.

var rows: DataFrame.Rows

The entire data frame as a collection of rows.

var base: DataFrame

The underlying data frame.

func containsColumn&lt;T>(String, T.Type) -> Bool

Returns a Boolean value indicating whether the data frame contains a column.

