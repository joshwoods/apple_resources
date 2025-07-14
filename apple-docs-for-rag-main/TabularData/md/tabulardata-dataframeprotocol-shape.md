

- TabularData
- DataFrameProtocol
-  shape 

Instance Property

# shape

The number or rows and columns of the data frame type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var shape: (rows: Int, columns: Int) { get }
```

**Required**

## Parameters 

`rows`  

The number of rows in the data frame type.

`columns`  

The number of columns in the data frame type.

## See Also

### Inspecting a Data Frame Type

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var columns: [Self.ColumnType]

The columns of the underlying data frame.

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

