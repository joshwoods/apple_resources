

- TabularData
-  AnyColumnProtocol 

Protocol

# AnyColumnProtocol

A type that represents a type-erased column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol AnyColumnProtocol
```

## Overview

`AnyColumnProtocol` defines the common functionality for type-erased column types. Its typed counterpart is ColumnProtocol.

## Topics

### Inspecting a Type-Erased Column Type

var name: String

The name of the column type.

**Required**

var count: Int

The number of elements in the column type.

**Required**

var wrappedElementType: any Any.Type

The underlying type of the column type’s elements.

**Required**

### Retrieving Elements

subscript(Int) -> Any?

Retrieves an element at a position in the column type.

**Required**

subscript(Range&lt;Int>) -> AnyColumnSlice

Retrieves a contiguous subrange of the column type’s elements.

**Required**

## Relationships

### Conforming Types

- AnyColumn
- AnyColumnSlice

## See Also

### Type-Erased Columns

struct AnyColumn

A type-erased column.

struct AnyColumnSlice

A type-erased column slice.

protocol AnyColumnPrototype

A prototype that creates type-erased columns.

