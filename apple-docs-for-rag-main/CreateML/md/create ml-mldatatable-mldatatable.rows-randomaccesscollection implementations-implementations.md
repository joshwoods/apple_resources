

- Create ML
- MLDataTable
- MLDataTable.Rows
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: Int

The DataTable’s “past the end” position—that is, the position one greater than the last valid subscript argument.

var startIndex: Int

The position of the first row in a nonempty DataTable. If the DataTable is empty, `startIndex` is equal to `endIndex`.

### Instance Methods

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

### Subscripts

subscript(Int) -> MLDataTable.Rows.Element

Subscript by index. This returns a row in the data table.

### Type Aliases

typealias Element

The Element of a DataTable is a Row. This is represented as a Dictionary-like type containing all Column names and their corresponding values.

