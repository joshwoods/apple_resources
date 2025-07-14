

- TabularData
- FilledColumn
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Generates a column by multiplying each element in a column by a value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func * (lhs: Self, rhs: Self.Element) -> Column
```

Available when `Element` conforms to `Numeric`.

## Parameters 

`lhs`  

A column type.

`rhs`  

A value of the same type as the column.

## Return Value

A new column.

## See Also

### Generating a Column by Multiplying a Value

static func * (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by multiplying a value by each element in a column.

