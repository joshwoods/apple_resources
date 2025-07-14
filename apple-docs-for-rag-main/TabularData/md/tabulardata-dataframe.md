

- TabularData
-  DataFrame 

Structure

# DataFrame

A collection that arranges data in rows and columns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
@dynamicMemberLookup
struct DataFrame
```

## Topics

### Creating a Data Frame

init()

Creates an empty data frame with no rows or columns.

init&lt;S>(columns: S)

Creates a new data frame from a sequence of columns.

init(dictionaryLiteral: (String, [Any?])...)

Creates a data frame from a dictionary literal.

### Creating a Data Frame from Other Data Frames

init(DataFrame.Slice)

Creates a new data frame with a slice of rows from another data frame.

struct Slice

A set of a data frame’s rows you create by using a method from a data frame instance or another data frame slice.

### Creating a Data Frame from a JSON File

init(contentsOfJSONFile: URL, columns: [String]?, types: [String : JSONType], options: JSONReadingOptions) throws

Creates a data frame by reading a JSON file.

init(jsonData: Data, columns: [String]?, types: [String : JSONType], options: JSONReadingOptions) throws

Creates a data frame by converting JSON data.

enum JSONType

Represents the value types in a JSON file.

struct JSONReadingOptions

A set of JSON file-reading options.

### Creating a Data Frame from a CSV

init(contentsOfCSVFile: URL, columns: [String]?, rows: Range&lt;Int>?, types: [String : CSVType], options: CSVReadingOptions) throws

Creates a data frame from a CSV file.

init(csvData: Data, columns: [String]?, rows: Range&lt;Int>?, types: [String : CSVType], options: CSVReadingOptions) throws

Creates a data frame from CSV data.

enum CSVType

Represents the value types in a CSV file.

struct CSVReadingOptions

A set of CSV file-reading options.

### Creating a Data Frame from Turi Create Types

init(contentsOfSFrameDirectory: URL, columns: [String]?, rows: Range&lt;Int>?) throws

Creates a data frame from a Turi Create scalable data frame.

struct ShapedData

A collection type that represents multidimensional data in a data frame element.

### Inspecting a Data Frame

var isEmpty: Bool

A Boolean that indicates whether the data frame type is empty.

var shape: (rows: Int, columns: Int)

The number of rows and columns in the data frame.

var columns: [AnyColumn]

The entire data frame as a collection of columns.

var rows: DataFrame.Rows

The entire data frame as a collection of rows.

struct Rows

A collection of rows in a data frame.

var base: DataFrame

The underlying data frame.

func containsColumn&lt;T>(String, T.Type) -> Bool

Returns a Boolean value indicating whether the data frame contains a column.

### Sorting a Data Frame

func sort(on: String, order: Order)

Arranges the rows of a data frame according to a column that you select by its name.

func sort&lt;T>(on: String, T.Type, order: Order)

Arranges the rows of a data frame according to a column that you select by its name and type.

func sort&lt;T>(on: String, T.Type, by: (T, T) throws -> Bool) rethrows

Arranges the rows of a data frame according to a column that you select by its name and type, with a predicate.

func sort&lt;T>(on: ColumnID&lt;T>, by: (T, T) throws -> Bool) rethrows

Arranges the rows of a data frame according to a column that you select by its column identifier, with a predicate.

func sort&lt;T>(on: ColumnID&lt;T>, order: Order)

Arranges the rows of a data frame according to a column that you select by its column identifier.

func sort&lt;T0, T1>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, order: Order)

Arranges the rows of a data frame according to two columns that you select by their column identifiers.

func sort&lt;T0, T1, T2>(on: ColumnID&lt;T0>, ColumnID&lt;T1>, ColumnID&lt;T2>, order: Order)

Arranges the rows of a data frame according to three columns that you select by their column identifiers.

### Summarizing a Data Frame

func summary() -> DataFrame

Generates a data frame that summarizes the columns of the data frame.

func summary(of: String...) -> DataFrame

Generates a data frame that summarizes the columns you select by name.

func summary(ofColumns: Int...) -> DataFrame

Generates a data frame that summarizes the columns you select by index.

enum SummaryColumnIDs

The summary data frame column identifiers.

### Saving a Data Frame to a CSV Format

func writeCSV(to: URL, options: CSVWritingOptions) throws

Creates a CSV file with the contents of the data frame type.

func csvRepresentation(options: CSVWritingOptions) throws -> Data

Generates a CSV data instance of the data frame type.

struct CSVWritingOptions

A set of CSV file-writing options.

### Describing a Data Frame

var description: String

A text representation of the data frame.

var debugDescription: String

A text representation of the data frame suitable for debugging.

func description(options: FormattingOptions) -> String

Generates a text representation of the data frame type.

var customMirror: Mirror

A mirror that reflects the data frame.

### Comparing Data Frames

static func == (DataFrame, DataFrame) -> Bool

Returns a Boolean that indicates whether the data frames are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Hashing a Data Frame

func hash(into: inout Hasher)

Hashes the essential components of the data frame by feeding them into a hasher.

var hashValue: Int

The hash value.

### Initializers

init&lt;S, Feature, Annotation>(S, featuresColumnID: ColumnID&lt;Feature>, annotationsColumnID: ColumnID&lt;Annotation>) throws

Creates a data frame from a sequence of annotated features.

init&lt;each T>(contentsOfCSVFile: URL, columns: repeat ColumnID&lt;each T>, rows: Range&lt;Int>?, options: CSVReadingOptions) throws

Creates a data frame from a CSV file.

init&lt;each T>(csvData: Data, columns: repeat ColumnID&lt;each T>, rows: Range&lt;Int>?, options: CSVReadingOptions) throws

Creates a data frame from CSV data.

### Instance Methods

func containsColumn&lt;T>(ColumnID&lt;T>) -> Bool

Returns a Boolean value indicating whether the data frame contains a column matching a column ID.

func containsColumn(String) -> Bool

Returns a Boolean value indicating whether the data frame contains a column.

func loadRangedAnnotations&lt;Annotation>(parameters: DataFrameTemporalAnnotationParameters&lt;Annotation>, continueOnFailure: Bool) throws -> [AnnotatedFeature&lt;TemporalFileSegment, Annotation>]

Loads training examples from a data frame containing annotations.

func selecting(ColumnSelection) -> DataFrame

Generates a data frame that includes only the column selection.

### Type Aliases

typealias ColumnType

A type that conforms to the type-erased column protocol.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

DataFrameProtocol Implementations

Equatable Implementations

ExpressibleByDictionaryLiteral Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- DataFrameProtocol
- Equatable
- ExpressibleByDictionaryLiteral
- Hashable

## See Also

### Data Tables

protocol DataFrameProtocol

A type that represents a data frame.

