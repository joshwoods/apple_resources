

- Create ML
- MLUntypedColumn
-  \

Operator

# \

Creates a column of Booleans by testing whether the given value is less than each element in the given column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func  MLUntypedColumn
```

## Parameters 

`a`  

A value.

`b`  

A column.

## Return Value

A new column of Booleans if the column and value have the same underlying type; otherwise an invalid column.

## See Also

### Comparing a value with a column to generate an untyped column of booleans

static func == (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is equal to each element in the given column.

static func != (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is not equal to each element in the given column.

static func > (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is greater than each element in the given column.

static func &lt;= (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is less than or equal to each element in the given column.

static func >= (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is greater than or equal to each element in the given column.

