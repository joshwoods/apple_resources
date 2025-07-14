

- TabularData
-  FilledColumn 

Structure

# FilledColumn

A view on a column that replaces missing elements with a default value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct FilledColumn where Base : OptionalColumnProtocol
```

## Topics

### Inspecting a Column

var name: String

The name of the column.

### Finding an Element Index

func argmin() -> Base.Index?

Returns the index of the element with the lowest value.

func argmax() -> FilledColumn&lt;Base>.Index?

Returns the index of the element with the highest value.

### Accessing Elements

subscript(Base.Index) -> Base.WrappedElement

Retrieves an element at a position in the column type.

### Summarizing a Column

func summary() -> CategoricalSummary&lt;FilledColumn&lt;Base>.WrappedElement>

Generates a categorical summary of the filled column’s elements, including default values.

func numericSummary() -> NumericSummary&lt;Double>

Generates a numeric summary of the integer column’s elements.

func numericSummary() -> NumericSummary&lt;Base.WrappedElement>

Generates a numeric summary of the floating-point column’s elements.

### Getting Statistical Values

func sum() -> FilledColumn&lt;Base>.Element

Returns the sum of the integer column’s elements.

func sum() -> FilledColumn&lt;Base>.Element

Returns the sum of the floating-point column’s elements.

func min() -> FilledColumn&lt;Base>.Element?

Returns the element with the lowest value.

func max() -> FilledColumn&lt;Base>.Element?

Returns the element with the highest value.

func mean() -> Double?

Returns the mean average of the integer column’s elements.

func mean() -> FilledColumn&lt;Base>.Element?

Returns the mean average of the floating-point column’s elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> Double?

Returns the standard deviation of the integer column’s elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> FilledColumn&lt;Base>.Element?

Returns the standard deviation of the floating-point column’s elements.

### Describing a Column

var description: String

A mirror that reflects the filled column.

var debugDescription: String

A text representation of the filled column suitable for debugging.

func description(options: FormattingOptions) -> String

Generates a string description of the filled column.

### Generating a Column by Combining Two Columns

static func + (Self, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column type to the corresponding elements of another.

static func - (Self, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column type from the corresponding elements of another.

static func * (Self, Self) -> Column&lt;Self.Element>

Generates a column by multiplying each element in a column type by the corresponding elements of another.

static func / (Self, Self) -> Column&lt;Self.Element>

Generates an integer column by dividing each element in a column type by the corresponding elements of another.

static func / (Self, Self) -> Column&lt;Self.Element>

Generates a floating-point column by dividing each element in a column type by the corresponding elements of another.

### Generating a Column by Adding a Value

static func + (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by adding a value to each element in a column.

static func + (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column to a value.

### Generating a Column by Subtracting a Value

static func - (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by subtracting a value from each element in a column.

static func - (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column from a value.

### Generating a Column by Multiplying a Value

static func * (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by multiplying each element in a column by a value.

static func * (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by multiplying a value by each element in a column.

### Generating a Column by Dividing a Value

static func / (Self, Self.Element) -> Column&lt;Self.Element>

Generates an integer column by dividing each element in a column by a value.

static func / (Self.Element, Self) -> Column&lt;Self.Element>

Generates an integer column by dividing a value by each element in a column.

static func / (Self, Self.Element) -> Column&lt;Self.Element>

Generates a floating-point column by dividing each element in a column by a value.

static func / (Self.Element, Self) -> Column&lt;Self.Element>

Generates a floating-point column by dividing a value by each element in a column.

### Comparing a Column with a Value

static func == (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is equal to a value.

static func == (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is equal to the corresponding element of a column type.

static func != (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type isn’t equal to a value.

static func != (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value isn’t equal to the corresponding element of a column type.

### Supporting Types

typealias Element

The type of the column’s elements that defines an associated type for the bidirectional collection protocol.

typealias WrappedElement

The type of the column’s elements that defines an associated type for the optional column protocol.

### Type Aliases

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

ColumnProtocol Implementations

CustomStringConvertible Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- ColumnProtocol
- Copyable
- CustomStringConvertible
- Sendable
- Sequence

## See Also

### Typed Columns

struct Column

A column in a data frame.

struct ColumnSlice

A collection that represents a selection of contiguous elements from a typed column.

struct DiscontiguousColumnSlice

A collection that represents a selection, potentially with gaps, of elements from a typed column.

protocol ColumnProtocol

A type that represents a column.

protocol OptionalColumnProtocol

A type that represents a column that has missing values.

