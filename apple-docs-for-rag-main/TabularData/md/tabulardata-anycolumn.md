

- TabularData
-  AnyColumn 

Structure

# AnyColumn

A type-erased column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct AnyColumn
```

## Overview

`AnyColumn` is a column type that conceals the type of its elements, unlike Column, its typed counterpart.

## Topics

### Inspecting a Type-Erased Column

var name: String

The name of the column.

var count: Int

The number of elements in the column.

var missingCount: Int

The number of missing elements in the column.

var wrappedElementType: any Any.Type

The underlying type of the column’s elements.

func isNil(at: Int) -> Bool

Returns a Boolean that indicates whether the element at the index is missing.

### Creating a Column of the Same Type

var prototype: any AnyColumnPrototype

A prototype that creates type-erased columns with the same underlying type as the column slice.

### Creating a Typed Column

func assumingType&lt;T>(T.Type) -> Column&lt;T>

Returns the underlying typed column.

### Adding Elements

func append(Any?)

Appends an optional element to the column.

func append(contentsOf: AnyColumn)

Appends the contents of another column to the column.

func append(contentsOf: AnyColumnSlice)

Appends the contents of a column slice to the column.

### Removing an Element

func remove(at: Int)

Removes an element from the column.

### Accessing Elements

subscript(Int) -> Any?

Accesses an element at an index.

subscript(Range&lt;Int>) -> AnyColumnSlice

Accesses a contiguous subrange of the elements.

### Creating a Slice of Unique Elements

func distinct() -> AnyColumnSlice

Generates a column slice that contains unique elements.

### Creating a Slice by Masking Elements

subscript&lt;C>(C) -> AnyColumnSlice

Returns a slice of the column by selecting elements with a collection of Booleans.

### Encoding a Column

func encode&lt;T, Encoder>(T.Type, using: Encoder) throws

Encodes each element of the column.

func encoded&lt;T, Encoder>(T.Type, using: Encoder) throws -> AnyColumn

Generates a column by encoding each element’s value.

### Decoding a Column

func decode&lt;T, Decoder>(T.Type, using: Decoder) throws

Decodes the data in each element of the column.

func decoded&lt;T, Decoder>(T.Type, using: Decoder) throws -> AnyColumn

Decodes data for each element of the column.

### Describing a Column

var description: String

A text representation of the column.

var debugDescription: String

A text representation of the column suitable for debugging.

var customMirror: Mirror

A mirror that reflects the column.

### Comparing Two Columns

static func == (AnyColumn, AnyColumn) -> Bool

Returns a Boolean that indicates whether the columns are equal.

static func != (Self, Self) -> Bool

Returns a Boolean value indicating whether two values are not equal.

### Hashing a Column

func hash(into: inout Hasher)

Hashes the essential components of the column by feeding them into a hasher.

### Instance Properties

var hashValue: Int

The hash value.

### Default Implementations

BidirectionalCollection Implementations

Collection Implementations

CustomDebugStringConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

Equatable Implementations

Hashable Implementations

MutableCollection Implementations

RandomAccessCollection Implementations

Sequence Implementations

## Relationships

### Conforms To

- AnyColumnProtocol
- BidirectionalCollection
- Collection
- Copyable
- CustomDebugStringConvertible
- CustomReflectable
- CustomStringConvertible
- Equatable
- Hashable
- MutableCollection
- RandomAccessCollection
- Sequence

## See Also

### Type-Erased Columns

struct AnyColumnSlice

A type-erased column slice.

protocol AnyColumnProtocol

A type that represents a type-erased column.

protocol AnyColumnPrototype

A prototype that creates type-erased columns.

