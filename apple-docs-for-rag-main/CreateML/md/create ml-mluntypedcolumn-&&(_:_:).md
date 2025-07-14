

- Create ML
- MLUntypedColumn
-  &&(\_:\_:) 

Operator

# &&(\_:\_:)

Creates a column of Booleans by performing a logical AND operation on each row of two columns of Booleans.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func && (a: MLUntypedColumn, b: MLUntypedColumn) -> MLUntypedColumn
```

## Parameters 

`a`  

A column.

`b`  

A column.

## Return Value

A new column of Booleans if the column and value have the same Boolean/integer underlying type; otherwise an invalid column.

## See Also

### Combining columns of booleans to generate an untyped column of booleans

static func || (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by performing a logical OR operation on each row of two columns of Booleans.

