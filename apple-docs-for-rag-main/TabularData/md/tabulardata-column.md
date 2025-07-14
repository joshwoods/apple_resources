

- TabularData
-  Column 

Structure

# Column

A column in a data frame.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct Column
```

## Overview

A column is a Collection that contains values of a specific type, including:

- Int

- Double

- String

Each element in a column is an Optional of the column’s type. Each `nil` element represents a missing value.

## Topics

### Creating a Column

init(name: String, capacity: Int)

Creates a column with a name and a capacity.

init(ColumnID&lt;WrappedElement>, capacity: Int)

Creates a column with a column identifier and a capacity.

init&lt;S>(name: String, contents: S)

Creates a column with a name and a sequence of nonoptional values.

init&lt;S>(name: String, contents: S)

Creates a column with a name and a sequence of optional values.

init&lt;S>(ColumnID&lt;S.Element>, contents: S)

Creates a column with an identifier and a sequence of nonoptional values.

init&lt;S>(ColumnID&lt;S.Element>, contents: S)

Creates a column with a column identifier and a sequence of optional values.

init(ColumnSlice&lt;WrappedElement>)

Creates a column from a column slice.

### Creating a Column of the Same Type

var prototype: any AnyColumnPrototype

A prototype that creates type-erased columns with the same underlying type as the column slice.

### Creating a Type-Erased Column

func eraseToAnyColumn() -> AnyColumn

Generates a type-erased copy of the column.

### Creating Transformed Columns

func map&lt;T>((Column&lt;WrappedElement>.Element) throws -> T?) rethrows -> Column&lt;T>

Creates a new column by applying a transformation to every element.

func mapNonNil&lt;T>((WrappedElement) throws -> T?) rethrows -> Column&lt;T>

Creates a new column by applying the transformation to every element that isn’t missing.

func filled(with: Self.WrappedElement) -> FilledColumn&lt;Self>

Generates a filled column by replacing missing elements with a value.

### Inspecting a Column

var name: String

The name of the column.

var count: Int

The number of elements in the column.

var missingCount: Int

The number of missing elements in the column.

typealias Element

The type of the column’s elements, which is an optional type of the column’s type.

var wrappedElementType: any Any.Type

The underlying type of the column’s elements.

### Transforming a Column

func transform((WrappedElement) throws -> WrappedElement) rethrows

Applies a transformation to every element that isn’t missing.

func transform((Column&lt;WrappedElement>.Element) throws -> Column&lt;WrappedElement>.Element) rethrows

Applies a transformation to every element in the column.

### Adding Elements

func append(WrappedElement)

Appends a nonoptional value to the column.

func append(Column&lt;WrappedElement>.Element)

Appends an optional value to the column.

func append&lt;S>(contentsOf: S)

Appends a sequence of nonoptional values to the column.

func append&lt;S>(contentsOf: S)

Appends a sequence of optional values to the column.

### Finding an Element Index

func argmin() -> Int?

Returns the index of the element with the lowest value, ignoring missing elements.

func argmax() -> Int?

Returns the index of the element with the highest value, ignoring missing elements.

### Removing an Element

func remove(at: Int)

Removes an element from the column.

### Accessing Elements

subscript(Int) -> Column&lt;WrappedElement>.Element

Accesses an element at an index.

subscript&lt;R>(R) -> ColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with a range expression.

subscript(Range&lt;Int>) -> ColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements.

### Creating a Slice of Unique Elements

func distinct() -> DiscontiguousColumnSlice&lt;WrappedElement>

Generates a discontiguous slice that contains unique elements.

### Creating a Slice by Masking Elements

subscript&lt;C>(C) -> DiscontiguousColumnSlice&lt;WrappedElement>

Returns a column slice that includes elements that correspond to a collection of Booleans.

### Encoding a Column

func encoded&lt;Encoder>(using: Encoder) throws -> Column&lt;Encoder.Output>

Generates a column by encoding each element’s value.

### Decoding a Column

func decoded&lt;T, Decoder>(T.Type, using: Decoder) throws -> Column&lt;T>

Generates a column by decoding each element’s data.

### Summarizing a Column

func summary() -> CategoricalSummary&lt;WrappedElement>

Generates a categorical summary of the column’s elements.

func numericSummary() -> NumericSummary&lt;Double>

Generates a numeric summary of the integer column’s elements.

func numericSummary() -> NumericSummary&lt;WrappedElement>

Generates a numeric summary of the floating-point column’s elements.

### Getting Statistical Values

func sum() -> WrappedElement

Returns the sum of the column’s elements, ignoring missing elements.

func min() -> Column&lt;WrappedElement>.Element

Returns the element with the lowest value, ignoring missing elements.

func max() -> Column&lt;WrappedElement>.Element

Returns the element with the highest value, ignoring missing elements.

func mean() -> Double?

Returns the mean average of the integer column’s elements, ignoring missing elements.

func mean() -> Column&lt;WrappedElement>.Element

Returns the mean average of the floating-point column’s elements, ignoring missing elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> Double?

Returns the standard deviation of the integer column’s elements, ignoring missing elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> Column&lt;WrappedElement>.Element

Returns the standard deviation of the floating-point column’s elements, ignoring missing elements.

### Describing a Column

var description: String

A text representation of the column.

var debugDescription: String

A text representation of the column suitable for debugging.

func description(options: FormattingOptions) -> String

Generates a string description of the optional column type.

var customMirror: Mirror

A mirror that reflects the column.

### Comparing Two Columns

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Modifying a Column with a Value

static func += (inout Column&lt;WrappedElement>, WrappedElement)

Modifies a column by adding a value to each element.

static func -= (inout Column&lt;WrappedElement>, WrappedElement)

Modifies a column by subtracting a value from each element.

static func *= (inout Column&lt;WrappedElement>, WrappedElement)

Modifies a column by multiplying each element by a value.

static func /= (inout Column&lt;WrappedElement>, WrappedElement)

Modifies an integer column by dividing each element by a value.

static func /= (inout Column&lt;WrappedElement>, WrappedElement)

Modifies a floating-point column by dividing each element by a value.

### Modifying a Column with a Collection of Values

static func += &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by adding each value in a collection to the corresponding element in the column.

static func += &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by adding each optional value in a collection to the corresponding element in the column.

static func -= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by subtracting each value in a collection from the corresponding element in the column.

static func -= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by subtracting each optional value in a collection from the corresponding element in the column.

static func *= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by multiplying each element in the column by the corresponding value in a collection.

static func *= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a column by multiplying each element in the column by the corresponding optional value in a collection.

static func /= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies an integer column by dividing each element in the column by the corresponding value in a collection.

static func /= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies an integer column by dividing each element in the column by the corresponding optional value in a collection.

static func /= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a floating-point column by dividing each element in the column by the corresponding value in a collection.

static func /= &lt;C>(inout Column&lt;WrappedElement>, C)

Modifies a floating-point column by dividing each element in the column by the corresponding optional value in a collection.

### Generating a Column by Combining Two Columns

static func + (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by adding each element in an optional column type to the corresponding elements of another.

static func - (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting each element in an optional column type from the corresponding elements of another.

static func * (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying each element in an optional column type by the corresponding elements of another.

static func / (Self, Self) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing each element in an optional column type by the corresponding elements of another.

static func / (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing each element in an optional column type by the corresponding elements of another.

### Generating a Column by Adding a Value

static func + (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by adding a value to each element in a column.

static func + (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column to a value.

static func + (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by adding a value to each element in an optional column.

static func + (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by adding each element in an optional column to a value.

### Generating a Column by Subtracting a Value

static func - (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by subtracting a value from each element in a column.

static func - (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column from a value.

static func - (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting a value from each element in an optional column type.

static func - (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting each element in an optional column from a value.

### Generating a Column by Multiplying a Value

static func * (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying each element in an optional column by a value.

static func * (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying a value by each element in an optional column type.

### Generating a Column by Dividing a Value

static func / (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing each element in an optional column by a value.

static func / (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing a value by each element in an optional column type.

static func / (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing each element in an optional column by a value.

static func / (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing a value by each element in an optional column type.

### Instance Methods

func withContiguousMutableStorageIfAvailable&lt;R>((inout UnsafeMutableBufferPointer&lt;WrappedElement>) throws -> R) rethrows -> R?

Call `body(buffer)`, where `buffer` provides access to the non-optional contiguous mutable storage of the entire column. If the column contains missing values, `body` is not called and `nil` is returned.

func withContiguousStorageIfAvailable&lt;R>((UnsafeBufferPointer&lt;WrappedElement>) throws -> R) rethrows -> R?

Call `body(buffer)`, where `buffer` provides access to the non-optional contiguous storage of the entire column. If the column contains missing values, `body` is not called and `nil` is returned.

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

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

Decodable Implementations

Encodable Implementations

Equatable Implementations

Hashable Implementations

MutableCollection Implementations

OptionalColumnProtocol Implementations

Sequence Implementations

## Relationships

### Conforms To

- BidirectionalCollection
- Collection
- ColumnProtocol
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Decodable
- Encodable
- Equatable
- Hashable
- MutableCollection
- OptionalColumnProtocol
- RandomAccessCollection
- Sendable
- Sequence

## See Also

### Typed Columns

struct ColumnSlice

A collection that represents a selection of contiguous elements from a typed column.

struct FilledColumn

A view on a column that replaces missing elements with a default value.

struct DiscontiguousColumnSlice

A collection that represents a selection, potentially with gaps, of elements from a typed column.

protocol ColumnProtocol

A type that represents a column.

protocol OptionalColumnProtocol

A type that represents a column that has missing values.

