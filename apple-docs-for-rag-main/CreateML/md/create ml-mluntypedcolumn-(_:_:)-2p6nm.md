

- Create ML
- MLUntypedColumn
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Creates a column by multiplying each element in the first column by the corresponding element in the second column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func * (a: MLUntypedColumn, b: MLUntypedColumn) -> MLUntypedColumn
```

## Parameters 

`a`  

A column.

`b`  

A column.

## Return Value

A new column if the columns have the same size and underlying type; otherwise an invalid column.

## See Also

### Combining columns to generate an untyped column

static func + (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column by adding each element in the first column to the corresponding element in the second column.

static func - (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column by subtracting each element in the second column from the corresponding element in the first column.

static func / (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column by dividing each element in the first column by the corresponding element in the second column.

