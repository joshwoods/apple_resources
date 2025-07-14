

- TabularData
-  OptionalColumnProtocol 

Protocol

# OptionalColumnProtocol

A type that represents a column that has missing values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol OptionalColumnProtocol : ColumnProtocol
```

## Overview

`OptionalColumnProtocol` defines the common functionality for column types that support missing values.

## Topics

### Filling an Optional Column

func filled(with: Self.WrappedElement) -> FilledColumn&lt;Self>

Generates a filled column by replacing missing elements with a value.

### Generating an Optional Column by Adding Two Columns

static func + (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by adding each element in an optional column type to the corresponding elements of another.

func + &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a column by adding each element in a column type to the corresponding elements of an optional column type.

func + &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a column by adding each element in an optional column type to the corresponding elements of a column type.

### Generating an Optional Column by Subtracting Two Columns

static func - (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting each element in an optional column type from the corresponding elements of another.

func - &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a column by subtracting each element in an optional column type from the corresponding elements of a column type.

func - &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a column by subtracting each element in a column type from the corresponding elements of an optional column.

### Generating an Optional Column by Multiplying Two Columns

static func * (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying each element in an optional column type by the corresponding elements of another.

func * &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a column by multiplying each element in an optional column type by the corresponding elements of a column type.

func * &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a column by multiplying each element in a column type by the corresponding elements of an optional column type.

### Generating an Optional Column by Dividing Two Columns

static func / (Self, Self) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing each element in an optional column type by the corresponding elements of another.

func / &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates an integer column by dividing each element in a column type by the corresponding elements of an optional column type.

func / &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates an integer column by dividing each element in an optional column type by the corresponding elements of a column type.

static func / (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing each element in an optional column type by the corresponding elements of another.

func / &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a floating-point column by dividing each element in a column type by the corresponding elements of an optional column type.

func / &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a floating-point column by dividing each element in an optional column type by the corresponding elements of a column type.

### Generating an Optional Column by Combining a Value

static func + (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by adding a value to each element in an optional column.

static func + (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by adding each element in an optional column to a value.

static func - (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting a value from each element in an optional column type.

static func - (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting each element in an optional column from a value.

static func * (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying each element in an optional column by a value.

static func * (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying a value by each element in an optional column type.

static func / (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing each element in an optional column by a value.

static func / (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing a value by each element in an optional column type.

static func / (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing each element in an optional column by a value.

static func / (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing a value by each element in an optional column type.

### Describing an Optional Column

func description(options: FormattingOptions) -> String

Generates a string description of the optional column type.

### Supporting Types

associatedtype WrappedElement

The type of the optional column type’s elements.

**Required**

## Relationships

### Inherits From

- BidirectionalCollection
- Collection
- ColumnProtocol
- Sequence

### Conforming Types

- Column
- ColumnSlice
- DiscontiguousColumnSlice

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

protocol ColumnProtocol

A type that represents a column.

