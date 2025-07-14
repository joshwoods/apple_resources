

- Create ML
- MLDataColumn
-  \

Operator

# \

Creates a column of Booleans by testing whether the given value is less than or equal to each element in the given column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func ) -> MLDataColumn
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`a`  

A value of the same type as the elements of the column.

`b`  

A column.

## Return Value

A new column of Booleans.

## See Also

### Comparing a value with a column to generate a column of booleans

static func == (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is equal to each element in the given column.

static func != (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is not equal to each element in the given column.

static func &lt; (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is less than each element in the given column.

static func > (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is greater than each element in the given column.

static func >= (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is greater than or equal to each element in the given column.

