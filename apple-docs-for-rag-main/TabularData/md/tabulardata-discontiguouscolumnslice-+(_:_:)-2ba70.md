

- TabularData
- DiscontiguousColumnSlice
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Generates a column by adding a value to each element in an optional column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func + (lhs: Self, rhs: Self.WrappedElement) -> Column where Self.WrappedElement : AdditiveArithmetic
```

## Parameters 

`lhs`  

An optional column type.

`rhs`  

A value of the same type as the optional column.

## Return Value

A new column.

## See Also

### Generating a Column by Adding a Value

static func + (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by adding a value to each element in a column.

static func + (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column to a value.

static func + (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by adding each element in an optional column to a value.

