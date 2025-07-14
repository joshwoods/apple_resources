

- TabularData
- DiscontiguousColumnSlice
-  /(\_:\_:) 

Operator

# /(\_:\_:)

Generates an integer column by dividing a value by each element in an optional column type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func / (lhs: Self.WrappedElement, rhs: Self) -> Column
```

Available when `WrappedElement` conforms to `BinaryInteger`.

## Parameters 

`lhs`  

A value of the same type as the optional column’s type.

`rhs`  

An optional column type.

## Return Value

A new column.

## See Also

### Generating a Column by Dividing a Value

static func / (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing each element in an optional column by a value.

static func / (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing each element in an optional column by a value.

static func / (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing a value by each element in an optional column type.

