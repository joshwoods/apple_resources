

- Create ML
- MLUntypedColumn
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Creates a column by multiplying the given value by each element of the given column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func * (a: any MLDataValueConvertible, b: MLUntypedColumn) -> MLUntypedColumn
```

## Parameters 

`a`  

An value.

`b`  

A column.

## Return Value

A new column if the column and value have the same underlying type; otherwise an invalid column.

## See Also

### Combining a value with a column to generate an untyped column

static func + (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column by adding the given value to each element of the given column.

static func - (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column by subtracting each element of the given column from the given value.

static func / (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column by dividing the given value by each element of the given column.

