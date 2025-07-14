

- TabularData
- ColumnProtocol
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Generates a column by multiplying each element in a column type by the corresponding elements of another.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func * (lhs: Self, rhs: Self) -> Column
```

Available when `Element` conforms to `Numeric`.

## Parameters 

`lhs`  

A column type.

`rhs`  

Another column type.

## Return Value

A new column.

## See Also

### Generating a Column by Multiplying Two Columns

func * &lt;L, R>(L, R) -> Column&lt;L.Element>

Generates a column by multiplying each element in a column type by the corresponding elements of an optional column type.

func * &lt;L, R>(L, R) -> Column&lt;R.Element>

Generates a column by multiplying each element in an optional column type by the corresponding elements of a column type.

