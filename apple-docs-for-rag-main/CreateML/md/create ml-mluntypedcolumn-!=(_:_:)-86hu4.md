

- Create ML
- MLUntypedColumn
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Creates a column of Booleans by testing whether each element in the first column is not equal to the corresponding element in the second column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func != (a: MLUntypedColumn, b: MLUntypedColumn) -> MLUntypedColumn
```

## Parameters 

`a`  

A column.

`b`  

A column.

## Return Value

A new column of Booleans if the columns have the same size and underlying type; otherwise an invalid column.

## See Also

### Comparing columns to generate an untyped column of booleans

static func == (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is equal to the corresponding element in the second column.

static func > (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is greater than the corresponding element in the second column.

static func &lt; (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is less than the corresponding element in the second column.

static func &lt;= (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is less than or equal to the corresponding element in the second column.

static func >= (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is greater than or equal to the corresponding element in the second column.

