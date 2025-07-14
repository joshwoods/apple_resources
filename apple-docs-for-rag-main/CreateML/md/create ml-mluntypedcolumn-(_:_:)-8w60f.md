

- Create ML
- MLUntypedColumn
-  \

Operator

# \

Creates a column of Booleans by testing whether each element in the given column is less than the given value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func  MLUntypedColumn
```

## Parameters 

`a`  

A column.

`b`  

A value.

## Return Value

A new column of Booleans if the column and value have the same underlying type; otherwise an invalid column.

## See Also

### Comparing a column with a value to generate an untyped column of booleans

static func == (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is equal to the given value.

static func != (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is not equal to the given value.

static func > (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is greater than the given value.

static func &lt;= (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is less than or equal to the given value.

static func >= (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is greater than or equal to the given value.

