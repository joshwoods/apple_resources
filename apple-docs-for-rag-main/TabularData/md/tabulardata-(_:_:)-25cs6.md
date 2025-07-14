

- TabularData
-  -(\_:\_:) 

Operator

# -(\_:\_:)

Generates a column by subtracting each element in an optional column type from the corresponding elements of a column type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func - (lhs: L, rhs: R) -> Column where L : ColumnProtocol, R : OptionalColumnProtocol, L.Element : AdditiveArithmetic, L.Element == R.WrappedElement
```

## Parameters 

`lhs`  

A column type.

`rhs`  

An optional column type.

## Return Value

A new column with the same type as the left column.

## See Also

### Generating a Column by Subtracting Two Columns

static func - (Self, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column type from the corresponding elements of another.

func - &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a column by subtracting each element in a column type from the corresponding elements of an optional column.

