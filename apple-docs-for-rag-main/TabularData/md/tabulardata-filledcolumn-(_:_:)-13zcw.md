

- TabularData
- FilledColumn
-  -(\_:\_:) 

Operator

# -(\_:\_:)

Generates a column by subtracting a value from each element in a column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func - (lhs: Self, rhs: Self.Element) -> Column where Self.Element : AdditiveArithmetic
```

## Parameters 

`lhs`  

A column type.

`rhs`  

A value of the same type as the column.

## Return Value

A new column.

## See Also

### Generating a Column by Subtracting a Value

static func - (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column from a value.

