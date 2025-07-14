

- TabularData
-  ColumnProtocol 

Protocol

# ColumnProtocol

A type that represents a column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol ColumnProtocol : BidirectionalCollection
```

## Overview

`ColumnProtocol` defines the common functionality for typed column types. Its type-erased counterpart is AnyColumnProtocol.

## Topics

### Inspecting a Column Type

var name: String

The name of the column.

**Required**

### Generating a Column by Adding Two Columns

static func + (Self, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column type to the corresponding elements of another.

func + &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a column by adding each element in a column type to the corresponding elements of an optional column type.

func + &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a column by adding each element in an optional column type to the corresponding elements of a column type.

### Generating a Column by Subtracting Two Columns

static func - (Self, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column type from the corresponding elements of another.

func - &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a column by subtracting each element in an optional column type from the corresponding elements of a column type.

func - &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a column by subtracting each element in a column type from the corresponding elements of an optional column.

### Generating a Column by Multiplying Two Columns

static func * (Self, Self) -> Column&lt;Self.Element>

Generates a column by multiplying each element in a column type by the corresponding elements of another.

func * &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a column by multiplying each element in a column type by the corresponding elements of an optional column type.

func * &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a column by multiplying each element in an optional column type by the corresponding elements of a column type.

### Generating a Column by Dividing Two Columns

static func / (Self, Self) -> Column&lt;Self.Element>

Generates an integer column by dividing each element in a column type by the corresponding elements of another.

func / &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates an integer column by dividing each element in a column type by the corresponding elements of an optional column type.

func / &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates an integer column by dividing each element in an optional column type by the corresponding elements of a column type.

static func / (Self, Self) -> Column&lt;Self.Element>

Generates a floating-point column by dividing each element in a column type by the corresponding elements of another.

func / &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a floating-point column by dividing each element in a column type by the corresponding elements of an optional column type.

func / &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a floating-point column by dividing each element in an optional column type by the corresponding elements of a column type.

### Generating a Column by Combining a Value

static func + (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by adding a value to each element in a column.

static func + (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column to a value.

static func - (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column from a value.

static func - (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by subtracting a value from each element in a column.

static func * (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by multiplying each element in a column by a value.

static func * (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by multiplying a value by each element in a column.

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

### Operators

static func > (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is greater than the corresponding element of a column type.

static func &lt; (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is less than the corresponding element of a column type.

static func &lt; (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is less than a value.

static func > (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is greater than a value.

static func &lt;= (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is less than or equal to the corresponding element of a column type.

static func >= (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is greater than or equal to a value.

static func >= (Self.Element, Self) -> [Bool]

Returns a Boolean array that indicates whether the value is greater than or equal to the corresponding element of a column type.

static func &lt;= (Self, Self.Element) -> [Bool]

Returns a Boolean array that indicates whether the corresponding element of a column type is less than or equal to a value.

## Relationships

### Inherits From

- BidirectionalCollection
- Collection
- Sequence

### Inherited By

- OptionalColumnProtocol

### Conforming Types

- Column
- ColumnSlice
- DiscontiguousColumnSlice
- FilledColumn

## See Also

### Typed Columns

struct Column

A column in a data frame.

struct ColumnSlice

A collection that represents a selection of contiguous elements from a typed column.

struct FilledColumn

A view on a column that replaces missing elements with a default value.

struct DiscontiguousColumnSlice

A collection that represents a selection, potentially with gaps, of elements from a typed column.

protocol OptionalColumnProtocol

A type that represents a column that has missing values.

