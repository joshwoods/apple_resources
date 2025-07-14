

- Create ML
- MLDataColumn
-  !=(\_:\_:) 

Operator

# !=(\_:\_:)

Creates a column of Booleans by testing whether each element in the given column is not equal to the given value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func != (a: MLDataColumn, b: Element) -> MLDataColumn
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`a`  

A column.

`b`  

A value of the same type as the elements of the column.

## Return Value

A new column of Booleans.

## See Also

### Comparing a column with a value to generate a column of booleans

static func == (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is equal to the given value.

static func &lt; (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is less than the given value.

static func &lt;= (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is less than or equal to the given value.

static func > (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is greater than the given value.

static func >= (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is greater than or equal to the given value.

