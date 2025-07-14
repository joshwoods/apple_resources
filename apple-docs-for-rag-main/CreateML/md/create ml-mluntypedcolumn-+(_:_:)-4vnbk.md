

- Create ML
- MLUntypedColumn
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Creates a column by adding each element of the given column to the given value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func + (a: MLUntypedColumn, b: any MLDataValueConvertible) -> MLUntypedColumn
```

## Parameters 

`a`  

An column.

`b`  

A value.

## Return Value

A new column if the column and value have the same underlying type; otherwise an invalid column.

## See Also

### Combining a column with a value to generate an untyped column

static func - (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column by subtracting the given value from each element of the given column.

static func * (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column by multiplying each element of the given column by the given value.

static func / (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column by dividing each element of the given column by the given value.

