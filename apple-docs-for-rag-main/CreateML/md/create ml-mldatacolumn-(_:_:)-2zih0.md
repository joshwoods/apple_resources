

- Create ML
- MLDataColumn
-  \*(\_:\_:) 

Operator

# \*(\_:\_:)

Creates a column of integers by multiplying each element of the given column by the given integer.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func * (a: MLDataColumn, b: Int) -> MLDataColumn
```

Available when `Element` is `Int`.

## Parameters 

`a`  

A column of integers.

`b`  

An integer.

## Return Value

A new column of integers.

## See Also

### Combining a column with a value to generate a column

static func + (MLDataColumn&lt;Int>, Int) -> MLDataColumn&lt;Int>

Creates a column of integers by adding each element of the given column to the given integer.

static func + (MLDataColumn&lt;Double>, Double) -> MLDataColumn&lt;Double>

Creates a column of doubles by adding each element of the given column to the given double.

static func - (MLDataColumn&lt;Int>, Int) -> MLDataColumn&lt;Int>

Creates a column of integers by subtracting the given integer from each element of the given column.

static func - (MLDataColumn&lt;Double>, Double) -> MLDataColumn&lt;Double>

Creates a column of doubles by subtracting the given double from each element of the given column.

static func * (MLDataColumn&lt;Double>, Double) -> MLDataColumn&lt;Double>

Creates a column of doubles by multiplying each element of the given column by the given double.

static func / (MLDataColumn&lt;Int>, Int) -> MLDataColumn&lt;Int>

Creates a column of integers by dividing each element of the given column by the given integer.

static func / (MLDataColumn&lt;Double>, Double) -> MLDataColumn&lt;Double>

Creates a column of doubles by dividing each element of the given column by the given double.

