

- TabularData
- FilledColumn
-  /(\_:\_:) 

Operator

# /(\_:\_:)

Generates an integer column by dividing each element in a column type by the corresponding elements of another.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func / (lhs: Self, rhs: Self) -> Column
```

Available when `Element` conforms to `BinaryInteger`.

## Parameters 

`lhs`  

A column type.

`rhs`  

Another column type.

## Return Value

A new column.

## See Also

### Generating a Column by Combining Two Columns

static func + (Self, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column type to the corresponding elements of another.

static func - (Self, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column type from the corresponding elements of another.

static func * (Self, Self) -> Column&lt;Self.Element>

Generates a column by multiplying each element in a column type by the corresponding elements of another.

static func / (Self, Self) -> Column&lt;Self.Element>

Generates a floating-point column by dividing each element in a column type by the corresponding elements of another.

