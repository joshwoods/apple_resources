

- Create ML
- MLDataColumn
-  -(\_:\_:) 

Operator

# -(\_:\_:)

Creates a column of integers by subtracting each element in the second column from the corresponding element in the first column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func - (a: MLDataColumn, b: MLDataColumn) -> MLDataColumn
```

Available when `Element` is `Int`.

## Parameters 

`a`  

A column of integers.

`b`  

A column of integers.

## Return Value

A new column of integers if the columns are the same size; otherwise an invalid column.

## See Also

### Combining columns to generate a column

static func + (MLDataColumn&lt;Int>, MLDataColumn&lt;Int>) -> MLDataColumn&lt;Int>

Creates a column of integers by adding each element in the first column to the corresponding element in the second column.

static func + (MLDataColumn&lt;Double>, MLDataColumn&lt;Double>) -> MLDataColumn&lt;Double>

Creates a column of doubles by adding each element in the first column to the corresponding element in the second column.

static func - (MLDataColumn&lt;Double>, MLDataColumn&lt;Double>) -> MLDataColumn&lt;Double>

Creates a column of doubles by subtracting each element in the second column from the corresponding element in the first column.

static func * (MLDataColumn&lt;Int>, MLDataColumn&lt;Int>) -> MLDataColumn&lt;Int>

Creates a column of integers by multiplying each element in the first column by the corresponding element in the second column.

static func * (MLDataColumn&lt;Double>, MLDataColumn&lt;Double>) -> MLDataColumn&lt;Double>

Creates a column of doubles by multiplying each element in the first column by the corresponding element in the second column.

static func / (MLDataColumn&lt;Int>, MLDataColumn&lt;Int>) -> MLDataColumn&lt;Int>

Creates a column of integers by dividing each element in the first column by the corresponding element in the second column.

static func / (MLDataColumn&lt;Double>, MLDataColumn&lt;Double>) -> MLDataColumn&lt;Double>

Creates a column of doubles by dividing each element in the first column by the corresponding element in the second column.

