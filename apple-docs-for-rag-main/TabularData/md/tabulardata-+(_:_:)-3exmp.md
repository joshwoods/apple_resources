

- TabularData
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Generates a column by adding each element in an optional column type to the corresponding elements of a column type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func + (lhs: L, rhs: R) -> Column where L : OptionalColumnProtocol, R : ColumnProtocol, L.WrappedElement : AdditiveArithmetic, L.WrappedElement == R.Element
```

## Parameters 

`lhs`  

An optional column type.

`rhs`  

A column type.

## Return Value

A new column with the same type as the right column.

## See Also

### Generating a Column by Adding Two Columns

static func + (Self, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column type to the corresponding elements of another.

func + &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a column by adding each element in a column type to the corresponding elements of an optional column type.

