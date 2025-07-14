

- TabularData
-  AnyColumnPrototype 

Protocol

# AnyColumnPrototype

A prototype that creates type-erased columns.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
protocol AnyColumnPrototype
```

## Topics

### Naming a Prototype Column

var name: String

The name of the column.

**Required**

### Creating Columns

func makeColumn(capacity: Int) -> AnyColumn

Creates a type-erased column.

**Required**

## See Also

### Type-Erased Columns

struct AnyColumn

A type-erased column.

struct AnyColumnSlice

A type-erased column slice.

protocol AnyColumnProtocol

A type that represents a type-erased column.

