

- Create ML
- MLDataColumn
-  \

Operator

# \

Creates a column of Booleans by testing whether each element in the first column is less than the corresponding element in the second column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func , b: MLDataColumn) -> MLDataColumn
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`a`  

A column.

`b`  

A column.

## Return Value

A new column of Booleans if the columns are the same size; otherwise an invalid column.

## See Also

### Comparing columns to generate a column of booleans

static func == (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is equal to the corresponding element in the second column.

static func != (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is not equal to the corresponding element in the second column.

static func &lt;= (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is less than or equal to the corresponding element in the second column.

static func > (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is greater than the corresponding element in the second column.

static func >= (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is greater than or equal to the corresponding element in the second column.

