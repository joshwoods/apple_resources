

- Create ML
- MLDataColumn
-  +(\_:\_:) 

Operator

# +(\_:\_:)

Creates a column of integers by adding the given integer to each element of the given column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
static func + (a: Int, b: MLDataColumn) -> MLDataColumn
```

Available when `Element` is `Int`.

## Parameters 

`a`  

An integer.

`b`  

A column of integers.

## Return Value

A new column of integers.

## See Also

### Combining a value with a column to generate a column

static func + (Double, MLDataColumn&lt;Double>) -> MLDataColumn&lt;Double>

Creates a column of doubles by adding the given double to each element of the given column.

static func - (Int, MLDataColumn&lt;Int>) -> MLDataColumn&lt;Int>

Creates a column of integers by subtracting each element of the given column from the given integer.

static func - (Double, MLDataColumn&lt;Double>) -> MLDataColumn&lt;Double>

Creates a column of doubles by subtracting each element of the given column from the given double.

static func * (Int, MLDataColumn&lt;Int>) -> MLDataColumn&lt;Int>

Creates a column of integers by multiplying the given integer by each element of the given column.

static func * (Double, MLDataColumn&lt;Double>) -> MLDataColumn&lt;Double>

Creates a column of doubles by multiplying the given double by each element of the given column.

static func / (Int, MLDataColumn&lt;Int>) -> MLDataColumn&lt;Int>

Creates a column of integers by dividing the given integer by each element of the given column.

static func / (Double, MLDataColumn&lt;Double>) -> MLDataColumn&lt;Double>

Creates a column of doubles by dividing the given double by each element of the given column.

