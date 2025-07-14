

- TabularData
- ColumnSlice
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Generates a column by multiplying each element in an optional column type by the corresponding elements of another.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func * (lhs: Self, rhs: Self) -> Column
```

Available when `WrappedElement` conforms to `Numeric`.

## Parameters 

`lhs`  

An optional column type.

`rhs`  

Another optional column type.

## Return Value

A new column.

## See Also

### Generating a Column by Combining Two Column Slices

static func + (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by adding each element in an optional column type to the corresponding elements of another.

static func - (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a column by subtracting each element in an optional column type from the corresponding elements of another.

static func / (Self, Self) -> Column&lt;Self.WrappedElement>

Generates an integer column by dividing each element in an optional column type by the corresponding elements of another.

static func / (Self, Self) -> Column&lt;Self.WrappedElement>

Generates a floating-point column by dividing each element in an optional column type by the corresponding elements of another.

