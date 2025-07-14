

- TabularData
- DataFrameProtocol
-  columns 

Instance Property

# columns

The columns of the underlying data frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var columns: [Self.ColumnType] { get }
```

**Required**

## See Also

### Inspecting a Data Frame Type

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number or rows and columns of the data frame type.

**Required**

associatedtype ColumnType : AnyColumnProtocol

A type that conforms to the type-erased column protocol.

**Required**

var rows: DataFrame.Rows

The rows of the underlying data frame.

**Required**

struct Rows

A collection of rows in a data frame.

var base: DataFrame

The underlying data frame.

**Required**

