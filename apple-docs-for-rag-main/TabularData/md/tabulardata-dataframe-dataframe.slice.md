

- TabularData
- DataFrame
-  DataFrame.Slice 

Structure

# DataFrame.Slice

A set of a data frame’s rows you create by using a method from a data frame instance or another data frame slice.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@dynamicMemberLookup
struct Slice
```

## Overview

A slice is an arbitrary set of rows from a data frame. For example, a slice might contain rows 0–3, 5–9, and 101 from its underlying data frame.

## Topics

### Inspecting a Slice

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number of rows and columns in the slice.

var columns: [AnyColumnSlice]

The entire slice as a collection of columns.

var rows: DataFrame.Rows

The entire slice as a collection of rows.

var base: DataFrame

The underlying data frame.

### Creating a Slice by Selecting a Column

subscript&lt;T>(ColumnID&lt;T>) -> DiscontiguousColumnSlice&lt;T>

Returns a column you select by its column identifier.

subscript&lt;T>(column _: Int, T.Type) -> DiscontiguousColumnSlice&lt;T>

Returns a column you select by its index.

subscript&lt;T>(String, T.Type) -> DiscontiguousColumnSlice&lt;T>

Returns a column you select by its name and type.

subscript(String) -> AnyColumnSlice

Returns a column you select by its name.

subscript(dynamicMember _: String) -> AnyColumnSlice

Returns a column you select by its name to support dynamic-member lookup.

### Creating a Slice by Selecting Multiple Columns

subscript&lt;S>(S) -> DataFrame.Slice

Generates a data frame slice that includes the columns in a sequence of column names.

func selecting&lt;S>(columnNames: S) -> DataFrame.Slice

Generates a data frame slice that includes the columns you select with a sequence of names.

func selecting(columnNames: String...) -> DataFrame.Slice

Generates a data frame slice that includes the columns you select with a list of names.

### Creating a Slice by Selecting Rows

func prefix(Int) -> DataFrame.Slice

Returns a new slice that contains the initial elements of the original slice.

func prefix(upTo: Int) -> DataFrame.Slice

Returns a new slice that contains the initial elements of the original slice up to, but not including, the element at a position.

func prefix(through: Int) -> DataFrame.Slice

Returns a new slice that contains the initial elements of the original slice up to and including the element at a position.

func suffix(Int) -> DataFrame.Slice

Returns a new slice that contains the final elements of the original slice.

func suffix(from: Int) -> DataFrame.Slice

Returns a new slice that contains the final elements of the original slice beginning with the element at a position.

### Creating a Slice by Filtering Rows

func filter&lt;T>(on: ColumnID&lt;T>, (T?) throws -> Bool) rethrows -> DataFrame.Slice

Returns a selection of rows that satisfy a predicate in the columns you select by column identifier.

func filter&lt;T>(on: String, T.Type, (T?) throws -> Bool) rethrows -> DataFrame.Slice

Returns a selection of rows that satisfy a predicate in the columns you select by name.

### Creating Two Slices by Splitting Rows

func randomSplit(by: Double, seed: Int?) -> (DataFrame.Slice, DataFrame.Slice)

Generates two data frame slices by randomly splitting the rows of the data table.

func randomSplit&lt;G>(by: Double, using: inout G) -> (DataFrame.Slice, DataFrame.Slice)

Generates two data frame slices by randomly splitting the rows of the data table type with a random-number generator.

### Creating Two Data Frames by Splitting Rows

func stratifiedSplit(on: String, by: Double, randomSeed: Int?) -> (DataFrame, DataFrame)

Generates two data frames by randomly splitting the rows of a column, which you select by its name, into strata.

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

func sorted&lt;T>(on: ColumnID&lt;T>, by: (T, T) throws -> Bool) rethrows -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to a column that you select by its column identifier, with a predicate.

### Creating a Data Frame by Sorting Multiple Columns

func sorted&lt;T0, T1>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to two columns that you select by their column identifiers.

func sorted&lt;T0, T1, T2>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>, order: Order) -> DataFrame

Generates a data frame by copying the data frame’s rows and then sorting the rows according to three columns that you select by their column identifiers.

### Creating a Data Frame by Joining with Another Data Frame

func joined&lt;R>(R, on: String, kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type with a common column you select by name.

func joined&lt;R>(R, on: (left: String, right: String), kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type along the columns that you select by name for both data frame types.

func joined&lt;R, T>(R, on: (left: ColumnID&lt;T>, right: ColumnID&lt;T>), kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type along the columns that you select by identifier for both data frame types.

func joined&lt;R, T>(R, on: ColumnID&lt;T>, kind: JoinKind) -> DataFrame

Generates a data frame by joining with another data frame type with a common column that you select by identifier.

### Grouping Rows

func grouped(by: String, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by name.

func grouped(by: ColumnID&lt;Date>, timeUnit: Calendar.Component) -> RowGrouping&lt;Int>

Creates a grouping of rows that the method selects by choosing unique units of time in a date column you select by column identifier.

func grouped&lt;InputKey, GroupingKey>(by: String, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by name.

func grouped&lt;InputKey, GroupingKey>(by: ColumnID&lt;InputKey>, transform: (InputKey?) -> GroupingKey?) -> RowGrouping&lt;GroupingKey>

Creates a grouping of rows that the method selects by choosing unique values the transform closure creates with elements of a column you select by column identifier.

struct RowGrouping

A collection of row selections that have the same value in a column.

func grouped(by: String) -> any RowGroupingProtocol

Creates a grouping of rows that the method selects by choosing unique values in a column.

func grouped&lt;T0, T1>(by: ColumnID&lt;T0>, ColumnID&lt;T1>) -> some RowGroupingProtocol

Creates a grouping from two columns of different types.

func grouped&lt;T0, T1, T2>(by: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>) -> some RowGroupingProtocol

Creates a grouping from three columns of different types.

protocol RowGroupingProtocol

A type that represents a collection of row selections that have the same value in a column.

### Summarizing a Slice

func summary() -> DataFrame

Generates a data frame that summarizes the columns of the data frame slice.

func summary(of: String...) -> DataFrame

Generates a data frame that summarizes the columns you select by name.

func summary(ofColumns: Int...) -> DataFrame

Generates a data frame that summarizes the columns you select by index.

enum SummaryColumnIDs

The summary data frame column identifiers.

### Saving a Slice to a CSV

func writeCSV(to: URL, options: CSVWritingOptions) throws

Creates a CSV file with the contents of the data frame type.

func csvRepresentation(options: CSVWritingOptions) throws -> Data

Generates a CSV data instance of the data frame type.

### Comparing Slices

static func == (DataFrame.Slice, DataFrame.Slice) -> Bool

Returns a Boolean that indicates whether the slices are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Describing a Slice

var description: String

A text representation of the data frame slice.

var debugDescription: String

A text representation of the data frame slice suitable for debugging.

func description(options: FormattingOptions) -> String

Generates a text representation of the data frame type.

var customMirror: Mirror

A mirror that reflects the data frame slice.

### Hashing a Slice

func hash(into: inout Hasher)

Hashes the essential components of the data frame slice by feeding them into a hasher.

### Type Aliases

typealias ColumnType

A type that conforms to the type-erased column protocol.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

DataFrameProtocol Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- DataFrameProtocol
- Equatable
- Hashable

## See Also

### Creating a Data Frame from Other Data Frames

init(DataFrame.Slice)

Creates a new data frame with a slice of rows from another data frame.

