

- TabularData
-  DiscontiguousColumnSlice 

Structure

# DiscontiguousColumnSlice

A collection that represents a selection, potentially with gaps, of elements from a typed column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct DiscontiguousColumnSlice
```

## Overview

A column slice contains only certain elements from its parent column. Create a slice by selecting certain elements. For example, use filter(_:) to create a slice that only includes elements with even values.

```
let slice = column.filter({ $0.isMultiple(of: 2) })
```

## Topics

### Creating a Column Slice

init(Column&lt;WrappedElement>)

Creates a slice with the contents of a column.

init(column: Column&lt;WrappedElement>, ranges: [Range&lt;Int>])

Creates a slice with the contents of a column.

### Creating a Slice of Unique Elements

func distinct() -> DiscontiguousColumnSlice&lt;WrappedElement>

Generates a discontiguous slice that contains unique elements.

### Creating a Type-Erased Slice

func eraseToAnyColumn() -> AnyColumnSlice

Generates a type-erased copy of the column slice.

### Creating a Column of the Same Type

var prototype: any AnyColumnPrototype

A prototype that creates type-erased columns with the same underlying type as the column slice.

### Creating Transformed Columns

func map&lt;T>((DiscontiguousColumnSlice&lt;WrappedElement>.Element) throws -> T?) rethrows -> Column&lt;T>

Creates a new column by applying a transformation to each element.

func filled(with: Self.WrappedElement) -> FilledColumn&lt;Self>

Generates a filled column by replacing missing elements with a value.

### Inspecting a Column Slice

var name: String

The name of the slice’s parent column.

var count: Int

The number of elements in the column slice.

var wrappedElementType: any Any.Type

The underlying type of the column’s elements.

func argmin() -> Int?

Returns the index of the element with the lowest value, ignoring missing elements.

func argmax() -> Int?

Returns the index of the element with the highest value, ignoring missing elements.

func isNil(at: Int) -> Bool

Returns a Boolean that indicates whether the element at the index is missing.

### Accessing Elements

subscript(Int) -> DiscontiguousColumnSlice&lt;WrappedElement>.Element

Accesses an element at an index.

subscript(Range&lt;Int>) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements.

subscript&lt;R>(R) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with a range expression.

subscript((UnboundedRange_) -> ()) -> DiscontiguousColumnSlice&lt;WrappedElement>

Accesses a contiguous range of elements with an unbounded range.

### Summarizing a Column Slice

func summary() -> CategoricalSummary&lt;WrappedElement>

Generates a categorical summary of the column slice’s elements.

func numericSummary() -> NumericSummary&lt;Double>

Generates a numeric summary of the integer column slice’s elements.

func numericSummary() -> NumericSummary&lt;WrappedElement>

Generates a numeric summary of the floating-point column slice’s elements.

### Getting Statistical Values

func sum() -> WrappedElement

Returns the sum of the column slice’s elements, ignoring missing elements.

func min() -> DiscontiguousColumnSlice&lt;WrappedElement>.Element

Returns the element with the lowest value, ignoring missing elements.

func max() -> DiscontiguousColumnSlice&lt;WrappedElement>.Element

Returns the element with the highest value, ignoring missing elements.

func mean() -> DiscontiguousColumnSlice&lt;WrappedElement>.Element

Returns the mean average of the floating-point slice’s elements, ignoring missing elements.

func mean() -> Double?

Returns the mean average of the integer slice’s elements, ignoring missing elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> Double?

Returns the standard deviation of the integer column slice’s elements, ignoring missing elements.

func standardDeviation(deltaDegreesOfFreedom: Int) -> DiscontiguousColumnSlice&lt;WrappedElement>.Element

Returns the standard deviation of the floating-point column slice’s elements, ignoring missing elements.

### Describing a Column Slice

var description: String

A text representation of the column slice.

var debugDescription: String

A text representation of the column slice suitable for debugging.

func description(options: FormattingOptions) -> String

Generates a string description of the optional column type.

var customMirror: Mirror

A mirror that reflects the column slice.

### Comparing Two Column Slices

static func == (DiscontiguousColumnSlice&lt;WrappedElement>, DiscontiguousColumnSlice&lt;WrappedElement>) -> Bool

Returns a Boolean that indicates whether the column slices are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Modifying a Column Slice with a Value

static func += (inout DiscontiguousColumnSlice&lt;WrappedElement>, WrappedElement)

Modifies a column slice by adding a value to each element.

static func -= (inout DiscontiguousColumnSlice&lt;WrappedElement>, WrappedElement)

Modifies a column slice by subtracting a value from each element.

static func *= (inout DiscontiguousColumnSlice&lt;WrappedElement>, WrappedElement)

Modifies a column slice by multiplying each element by a value.

static func /= (inout DiscontiguousColumnSlice&lt;WrappedElement>, WrappedElement)

Modifies an integer column slice by dividing each element by a value.

static func /= (inout DiscontiguousColumnSlice&lt;WrappedElement>, WrappedElement)

Modifies a floating-point column slice by dividing each element by a value.

### Modifying a Column Slice with a Collection of Values

static func += &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by adding each value in a collection to the corresponding element in the column.

static func += &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by adding each optional value in a collection to the corresponding element in the column.

static func -= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by subtracting each value in a collection from the corresponding element in the column.

static func -= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by subtracting each optional value in a collection from the corresponding element in the column.

static func *= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by multiplying each element in the column by the corresponding value in a collection.

static func *= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a column slice by multiplying each element in the column by the corresponding optional value in a collection.

static func /= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies an integer column slice by dividing each element in the column by the corresponding value in a collection.

static func /= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies an integer column slice by dividing each element in the column by the corresponding optional value in a collection.

static func /= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a floating-point column slice by dividing each element in the column by the corresponding value in a collection.

static func /= &lt;C>(inout DiscontiguousColumnSlice&lt;WrappedElement>, C)

Modifies a floating-point column slice by dividing each element in the column by the corresponding optional value in a collection.

### Generating a Column by Combining Two Column Slices

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

static func / (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing each element in an optional column by a value.

static func / (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing a value by each element in an optional column type.

static func / (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing a value by each element in an optional column type.

### Hashing a Column Slice

func hash(into: inout Hasher)

Hashes the essential components of the column slice by feeding them into a hasher.

### Supporting Types

typealias Element

The type of the column slice’s elements.

typealias Index

The type that represents a position in the column slice.

### Instance Properties

var missingCount: Int

The number of missing elements in the column slice.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

ColumnProtocol Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

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
- Equatable
- Hashable
- MutableCollection
- OptionalColumnProtocol
- Sendable
- Sequence

## See Also

### Typed Columns

struct Column

A column in a data frame.

struct ColumnSlice

A collection that represents a selection of contiguous elements from a typed column.

struct FilledColumn

A view on a column that replaces missing elements with a default value.

protocol ColumnProtocol

A type that represents a column.

protocol OptionalColumnProtocol

A type that represents a column that has missing values.

