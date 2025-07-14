

- TabularData
-  DataFrameProtocol 

Protocol

# DataFrameProtocol

A type that represents a data frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol DataFrameProtocol
```

## Topics

### Inspecting a Data Frame Type

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number or rows and columns of the data frame type.

**Required**

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

### Accessing Rows

subscript(Range&lt;Int>) -> DataFrame.Slice

Accesses a slice of the data frame type with an index range.

**Required** Default implementations provided.

subscript&lt;R>(R) -> DataFrame.Slice

Accesses rows of a data frame type with an index range expression.

### Creating Two Slices by Splitting Rows

func randomSplit(by: Double, seed: Int?) -> (DataFrame.Slice, DataFrame.Slice)

Generates two data frame slices by randomly splitting the rows of the data table.

func randomSplit&lt;G>(by: Double, using: inout G) -> (DataFrame.Slice, DataFrame.Slice)

Generates two data frame slices by randomly splitting the rows of the data table type with a random-number generator.

### Creating Two Data Frames by Splitting Rows

func stratifiedSplit(on: String, by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of a column, which you select by its name, into strata.

func stratifiedSplit(on: String..., by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of multiple columns, which you select by their names, into strata.

func stratifiedSplit&lt;T>(on: ColumnID&lt;T>, by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of a column, which you select by column identifier, into strata.

func stratifiedSplit&lt;T0, T1>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of two columns, which you select by column identifiers, into strata.

func stratifiedSplit&lt;T0, T1, T2>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>, by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of three columns, which you select by column identifiers, into strata.

### Creating a Data Frame by Sorting a Column

func sorted(on: String, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name.

func sorted&lt;T>(on: String, T.Type, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type.

func sorted&lt;T>(on: String, T.Type, by: (T, T) throws -> Bool) rethrows -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its name and type, with a predicate.

func sorted&lt;T>(on: ColumnID&lt;T>, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its column identifier.

func sorted&lt;T>(on: ColumnID&lt;T>, by: (T, T) throws -> Bool) rethrows -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its column identifier, with a predicate.

### Creating a Data Frame by Sorting Multiple Columns

func sorted&lt;T0, T1>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to two columns that you select by their column identifiers.

func sorted&lt;T0, T1, T2>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to three columns that you select by their column identifiers.

### Creating a Data Frame by Joining Another Data Frame

func joined&lt;R>(R, on: String, kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type with a common column you select by name.

func joined&lt;R>(R, on: (left: String, right: String), kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type along the columns that you select by name for both data frame types.

func joined&lt;R, T>(R, on: (left: ColumnID&lt;T>, right: ColumnID&lt;T>), kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type along the columns that you select by identifier for both data frame types.

func joined&lt;R, T>(R, on: ColumnID&lt;T>, kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type with a common column that you select by identifier.

enum JoinKind

An operation type that joins two data frame types.

### Creating a Row Grouping by a Column

func grouped&lt;GroupingKey>(by: ColumnID&lt;GroupingKey>) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values in a column.

func grouped(by: String, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by name.

func grouped(by: ColumnID&lt;Date>, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by column identifier.

func grouped&lt;InputKey, GroupingKey>(by: String, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by name.

func grouped&lt;InputKey, GroupingKey>(by: ColumnID&lt;InputKey>, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by column identifier.

### Creating a Row Grouping by Multiple Columns

func grouped(by: String...) -> some RowGroupingProtocol

Creates a grouping from multiple columns you select by name.

func grouped&lt;T>(by: ColumnID&lt;T>...) -> some RowGroupingProtocol

Creates a grouping from multiple columns that you select by column identifier.

func grouped&lt;T0, T1>(by: ColumnID&lt;T0>, ColumnID&lt;T1>) -> some RowGroupingProtocol

Creates a grouping from two columns of different types.

func grouped&lt;T0, T1, T2>(by: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>) -> some RowGroupingProtocol

Creates a grouping from three columns of different types.

### Saving a Data Frame Type to a CSV Format

func writeCSV(to: URL, options: CSVWritingOptions) throws

Creates a CSV file with the contents of the data frame type.

func csvRepresentation(options: CSVWritingOptions) throws -> Data

Generates a CSV data instance of the data frame type.

### Describing a Data Frame Type

func description(options: FormattingOptions) -> String

Generates a text representation of the data frame type.

### Instance Methods

func jsonRepresentation(options: JSONWritingOptions) throws -> Data

Generates a JSON data instance of the data frame.

func writeJSON(to: URL, options: JSONWritingOptions) throws

Creates a JSON file with the contents of the data frame.

## Relationships

### Conforming Types

- DataFrame
- DataFrame.Slice

## See Also

### Data Tables

struct DataFrame

A collection that arranges data in rows and columns.

