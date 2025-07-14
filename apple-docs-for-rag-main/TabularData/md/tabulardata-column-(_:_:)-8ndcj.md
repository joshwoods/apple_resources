

- TabularData
- Column
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Generates a column by multiplying each element in an optional column by a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func * (lhs: Self, rhs: Self.WrappedElement) -> Column
```

Available when `WrappedElement` conforms to `Numeric`.

## Parameters 

`lhs`  

An optional column type.

`rhs`  

A value of the same type as the optional column’s type.

## Return Value

A new column.

## See Also

### Generating a Column by Multiplying a Value

static func * (Self.WrappedElement, Self) -> Column&lt;Self.WrappedElement>

Generates a column by multiplying a value by each element in an optional column type.

