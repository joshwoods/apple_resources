

- TabularData
- DiscontiguousColumnSlice
-  -(\_:\_:) 

Operator

# -(\_:\_:)

Generates a column by subtracting each element in an optional column from a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func - (lhs: Self.WrappedElement, rhs: Self) -> Column where Self.WrappedElement : AdditiveArithmetic
```

## Parameters 

`lhs`  

A value of the same type as the optional column’s type.

`rhs`  

An optional column type.

## Return Value

A new column.

## See Also

### Generating a Column by Subtracting a Value

static func - (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by subtracting a value from each element in a column.

static func - (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column from a value.

static func - (Self, Self.WrappedElement) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting a value from each element in an optional column type.

