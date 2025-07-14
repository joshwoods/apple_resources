

- Create ML
-  MLDataColumn 

Structure

# MLDataColumn

A column of typed values in a data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct MLDataColumn where Element : MLDataValueConvertible
```

## Overview

A column is a homogenous collection of data values, similar to an Array. Columns are the main components of an MLDataTable and are designed to efficiently scale with large data sets.

Typically you use MLDataColumn, the typed equivalent to MLUntypedColumn, to work directly with the column’s element type. A data column has extra math and statistics functionality when its element type is Int or Double.

## Topics

### Creating a data column

init(repeating: Element, count: Int)

Creates a new column with a repeating element.

init(repeating: MLDataValue, count: Int)

Constructs a new Column containing the specified number of a single, repeated MLDataValue.

init&lt;S>(S)

Creates a new column from a given sequence of elements.

init()

Constructs an invalid Column.

### Creating a data column by converting another column

func map&lt;T>(to: T.Type) -> MLDataColumn&lt;T>

Creates a new column by converting this column to the given type.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of integers from a given column whose elements can be converted to integers.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of arrays of integers from a given column whose elements can be converted to an array of integers.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of doubles from a given column whose elements can be converted to doubles.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of arrays of doubles from a given column whose elements can be converted to an array of doubles.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of strings from a given column whose elements can be converted to strings.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of arrays of strings from a given column whose elements can be converted to an array of strings.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of machine learning sequences from a given column whose elements can be converted to sequences.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of machine learning dictionaries from a given column whose elements can be converted to dictionaries.

### Getting the number of elements

var count: Int

The number of elements in the column.

var isEmpty: Bool

### Getting an element

subscript(Int) -> Element

Accesses the element at the given row.

func element(at: Int) -> Element?

Accesses the element at the given index.

### Appending to a data column

func append(contentsOf: MLDataColumn&lt;Element>)

Appends the elements of the given column to the end of this column.

### Duplicating a column

func copy() -> MLDataColumn&lt;Element>

Returns a new MLDataColumn by copying the original MLDataColumn

### Sorting elements to generate a column

func sort(byIncreasingOrder: Bool) -> MLDataColumn&lt;Element>

Returns a new MLDataColumn containing values sorted by the specified order.

### Transforming elements to generate a column

func map&lt;T>((Element) -> T) -> MLDataColumn&lt;T>

Creates a new column by applying the given thread-safe transform to every non-missing element of this column.

func map&lt;T>((Element) -> T?) -> MLDataColumn&lt;T>

Creates a new column, potentially with missing values, by applying the given thread-safe transform to every non-missing element of this column.

func mapMissing&lt;T>((Element?) -> T?) -> MLDataColumn&lt;T>

Creates a new column, potentially with missing elements, by applying the given thread-safe transform to every element of the column, including missing elements.

### Masking elements to generate a column

subscript(MLDataColumn&lt;Bool>) -> MLDataColumn&lt;Element>

Creates a subset of the column by masking its elements with a column of Booleans.

subscript(MLUntypedColumn) -> MLDataColumn&lt;Element>

Returns a `MLDataColumn` containing only the elements for which the corresponding mask has a nonzero or non-default value.

### Discarding elements to generate a column

func dropMissing() -> MLDataColumn&lt;Element>

Creates a subset of the column by removing all elements without a value.

func dropDuplicates() -> MLDataColumn&lt;Element>

Creates a subset of the column by removing all duplicate elements.

### Selecting elements to generate a column

subscript(Range&lt;Int>) -> MLDataColumn&lt;Element>

Creates a subset of the column, given a range of elements.

subscript&lt;R>(R) -> MLDataColumn&lt;Element>

Creates a subset of the column, given a range expression of elements.

func prefix(Int) -> MLDataColumn&lt;Element>

Creates a subset of the column, given a number of initial elements.

func suffix(Int) -> MLDataColumn&lt;Element>

Creates a subset of the column, given a number of final elements.

### Filling in missing elements to generate a column

func fillMissing(with: Element) -> MLDataColumn&lt;Element>

Creates a modified copy of the column such that every missing element is replaced with the given value.

### Evaluating elements to generate a column

func materialize() throws -> MLDataColumn&lt;Element>

Creates a new column by immediately evaluating any lazily applied data processing operations stored in the column.

### Combining columns to generate a column

static func + (MLDataColumn&lt;Int>, MLDataColumn&lt;Int>) -> MLDataColumn&lt;Int>

Creates a column of integers by adding each element in the first column to the corresponding element in the second column.

static func + (MLDataColumn&lt;Double>, MLDataColumn&lt;Double>) -> MLDataColumn&lt;Double>

Creates a column of doubles by adding each element in the first column to the corresponding element in the second column.

static func - (MLDataColumn&lt;Int>, MLDataColumn&lt;Int>) -> MLDataColumn&lt;Int>

Creates a column of integers by subtracting each element in the second column from the corresponding element in the first column.

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

### Combining a column with a value to generate a column

static func + (MLDataColumn&lt;Int>, Int) -> MLDataColumn&lt;Int>

Creates a column of integers by adding each element of the given column to the given integer.

static func + (MLDataColumn&lt;Double>, Double) -> MLDataColumn&lt;Double>

Creates a column of doubles by adding each element of the given column to the given double.

static func - (MLDataColumn&lt;Int>, Int) -> MLDataColumn&lt;Int>

Creates a column of integers by subtracting the given integer from each element of the given column.

static func - (MLDataColumn&lt;Double>, Double) -> MLDataColumn&lt;Double>

Creates a column of doubles by subtracting the given double from each element of the given column.

static func * (MLDataColumn&lt;Int>, Int) -> MLDataColumn&lt;Int>

Creates a column of integers by multiplying each element of the given column by the given integer.

static func * (MLDataColumn&lt;Double>, Double) -> MLDataColumn&lt;Double>

Creates a column of doubles by multiplying each element of the given column by the given double.

static func / (MLDataColumn&lt;Int>, Int) -> MLDataColumn&lt;Int>

Creates a column of integers by dividing each element of the given column by the given integer.

static func / (MLDataColumn&lt;Double>, Double) -> MLDataColumn&lt;Double>

Creates a column of doubles by dividing each element of the given column by the given double.

### Combining a value with a column to generate a column

static func + (Int, MLDataColumn&lt;Int>) -> MLDataColumn&lt;Int>

Creates a column of integers by adding the given integer to each element of the given column.

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

### Comparing columns to generate a column of booleans

static func == (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is equal to the corresponding element in the second column.

static func != (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is not equal to the corresponding element in the second column.

static func &lt; (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is less than the corresponding element in the second column.

static func &lt;= (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is less than or equal to the corresponding element in the second column.

static func > (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is greater than the corresponding element in the second column.

static func >= (MLDataColumn&lt;Element>, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the first column is greater than or equal to the corresponding element in the second column.

### Comparing a column with a value to generate a column of booleans

static func == (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is equal to the given value.

static func != (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is not equal to the given value.

static func &lt; (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is less than the given value.

static func &lt;= (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is less than or equal to the given value.

static func > (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is greater than the given value.

static func >= (MLDataColumn&lt;Element>, Element) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether each element in the given column is greater than or equal to the given value.

### Comparing a value with a column to generate a column of booleans

static func == (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is equal to each element in the given column.

static func != (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is not equal to each element in the given column.

static func &lt; (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is less than each element in the given column.

static func &lt;= (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is less than or equal to each element in the given column.

static func > (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is greater than each element in the given column.

static func >= (Element, MLDataColumn&lt;Element>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by testing whether the given value is greater than or equal to each element in the given column.

### Combining columns of booleans to generate a column of booleans

static func &amp;&amp; (MLDataColumn&lt;Bool>, MLDataColumn&lt;Bool>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by performing a logical AND operation on each element in the first column with the corresponding element in the second column.

static func || (MLDataColumn&lt;Bool>, MLDataColumn&lt;Bool>) -> MLDataColumn&lt;Bool>

Creates a column of Booleans by performing a logical OR operation on each element in the first column with the corresponding element in the second column.

### Getting the min and max element values

func min() -> Int?

Returns the element with the lowest value in a column of integers.

func min() -> Double?

Returns the element with the lowest value in a column of doubles.

func max() -> Int?

Returns the element with the highest value in a column of integers.

func max() -> Double?

Returns the element with the highest value in a column of doubles.

### Getting sum, mean, and standard deviation values

func sum() -> Int?

Returns the sum of the elements in a column of integers.

func sum() -> Double?

Returns the sum of the elements in a column of doubles.

func mean() -> Double?

Returns the arithmetic mean of the elements in a column of integers.

func mean() -> Double?

Returns the arithmetic mean of the elements in a column of doubles.

func std() -> Double?

Returns the standard deviation of the elements in a column of integers.

func std() -> Double?

Returns the standard deviation of the elements in a column of doubles.

func stdev() -> Double?

Returns the standard deviation of the elements in a column of doubles.

func stdev() -> Double?

Standard deviation of the Elements in the MLDataColumn.

### Visualizing a column

func show() -> any MLStreamingVisualizable

Provides a visualization for the data in the column.

Deprecated

### Getting a description of a data column

var description: String

A text representation of the column.

var playgroundDescription: Any

A description of the column shown in a playground.

var debugDescription: String

A text representation of the column for debugging.

### Handling data column errors

var isValid: Bool

A Boolean value that indicates whether the column is valid.

var error: (any Error)?

The underlying error present when the column is invalid.

### Default Implementations

CustomDebugStringConvertible Implementations

CustomPlaygroundDisplayConvertible Implementations

CustomReflectable Implementations

CustomStringConvertible Implementations

## Relationships

### Conforms To

- Copyable
- CustomDebugStringConvertible
- CustomPlaygroundDisplayConvertible
- CustomReflectable
- CustomStringConvertible

## See Also

### Related Documentation

struct MLUntypedColumn

A column of untyped values in a data table.

### Adding columns

func addColumn&lt;Element>(MLDataColumn&lt;Element>, named: String)

Adds a data column to the table.

func addColumn(MLUntypedColumn, named: String)

Adds an untyped column to the table.

struct MLUntypedColumn

A column of untyped values in a data table.

