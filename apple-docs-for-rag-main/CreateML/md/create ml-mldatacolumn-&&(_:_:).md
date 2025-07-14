

- Create ML
- MLDataColumn
-  &&(\_:\_:) 

Operator

# &&(\_:\_:)

Creates a column of Booleans by performing a logical AND operation on each element in the first column with the corresponding element in the second column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func && (a: MLDataColumn, b: MLDataColumn) -> MLDataColumn
```

Available when `Element` is `Bool`.

## Parameters 

`a`  

A column of Booleans.

`b`  

A column of Booleans.

## Return Value

A new column of Booleans if the columns are the same size; otherwise an invalid column.

## See Also

### Combining columns of booleans to generate a column of booleans

static func || (MLDataColumn&lt;Bool>, MLDataColumn&lt;Bool>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by performing a logical OR operation on each element in the first column with the corresponding element in the second column.

