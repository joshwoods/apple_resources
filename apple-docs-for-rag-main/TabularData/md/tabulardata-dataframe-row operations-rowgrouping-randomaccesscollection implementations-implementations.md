

- TabularData
- DataFrame
- Row Operations
- RowGrouping
-  RandomAccessCollection Implementations 

API Collection

# RandomAccessCollection Implementations

## Topics

### Instance Properties

var endIndex: Int

The index of the final group in the row grouping.

var startIndex: Int

The index of the initial group in the row grouping.

### Instance Methods

func index(Self.Index, offsetBy: Int, limitedBy: Self.Index) -> Self.Index?

Returns an index that is the specified distance from the given index, unless that distance is beyond a given limiting index.

func index(after: Int) -> Int

Returns the index immediately after an element index.

func index(before: Int) -> Int

Returns the index immediately before an element index.

### Subscripts

subscript(Int) -> (key: GroupingKey?, group: DataFrame.Slice)

Retrieves a group at an index.

