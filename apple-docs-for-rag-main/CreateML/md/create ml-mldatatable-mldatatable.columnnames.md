

- Create ML
- MLDataTable
-  MLDataTable.ColumnNames 

Structure

# MLDataTable.ColumnNames

A collection of the names of the columns in a data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct ColumnNames
```

## Topics

### Manipulating indices

var startIndex: Int

The position of the first element in a nonempty collection.

var endIndex: Int

The collection’s “past the end” position—that is, the position one greater than the last valid subscript argument.

### Accessing columns

subscript(Int) -> String

Accesses the element at the specified position.

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

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomStringConvertible Implementations

Equatable Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomStringConvertible
- Equatable
- RandomAccessCollection
- Sequence

## See Also

### Getting information about a data table’s columns

var columnNames: MLDataTable.ColumnNames

The names of the columns in the data table.

var columnTypes: [String : MLDataValue.ValueType]

The type of the data in each column.

