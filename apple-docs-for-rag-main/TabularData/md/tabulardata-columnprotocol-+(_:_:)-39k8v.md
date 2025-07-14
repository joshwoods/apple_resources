

- TabularData
- ColumnProtocol
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Generates a column by adding a value to each element in a column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func + (lhs: Self, rhs: Self.Element) -> Column where Self.Element : AdditiveArithmetic
```

## Parameters 

`lhs`  

A column type.

`rhs`  

A value of the same type as the column.

## Return Value

A new column.

## See Also

### Generating a Column by Combining a Value

static func + (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by adding each element in a column to a value.

static func - (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by subtracting each element in a column from a value.

static func - (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by subtracting a value from each element in a column.

static func * (Self, Self.Element) -> Column&lt;Self.Element>

Generates a column by multiplying each element in a column by a value.

static func * (Self.Element, Self) -> Column&lt;Self.Element>

Generates a column by multiplying a value by each element in a column.

static func / (Self, Self.Element) -> Column&lt;Self.Element>

Generates an integer column by dividing each element in a column by a value.

static func / (Self.Element, Self) -> Column&lt;Self.Element>

Generates an integer column by dividing a value by each element in a column.

static func / (Self, Self.Element) -> Column&lt;Self.Element>

Generates a floating-point column by dividing each element in a column by a value.

static func / (Self.Element, Self) -> Column&lt;Self.Element>

Generates a floating-point column by dividing a value by each element in a column.

