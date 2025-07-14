

- Create ML
-  MLUntypedColumn 

Structure

# MLUntypedColumn

A column of untyped values in a data table.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
struct MLUntypedColumn
```

## Overview

A column is a homogenous collection of data values, similar to an Array. Columns are the main components of an MLDataTable and are designed to efficiently scale with large data sets.

Typically you use MLDataColumn, the typed equivalent to MLUntypedColumn, for its type-specific functionality.

Untyped columns are especially useful when:

- You’re initializing a data table with columns by using init(namedColumns:).

- You’re using columns of a non-Boolean type to filter a data table with subscript(_:).

- You don’t need to work directly with the underlying type.

Each element of an untyped column is an MLDataValue, and has an *underlying type* that conforms to MLDataValueConvertible. The underlying type is hidden from the Swift compiler and is what makes an MLUntypedColumn untyped. Using an untyped column allows you to quickly write type-agnostic code with Create ML.

```
let column = MLUntypedColumn([2, 3, 5, 7, 11])
let columnOver2 = column / 2 print(columnOver2)
/* Prints...
 ValueType: Double
 Values:        [1.0, 1.5, 2.5, 3.5, 5.5]
 */
```

However, by avoiding type safety at compile time, you expose your code to errors at runtime. When an error occurs during an operation, Create ML marks the product of that operation *invalid* by setting isValid to `false` and by setting error with a value. For example, using a slash (`/`) operator to divide a column of integers with a string produces an invalid column.

```
let column = MLUntypedColumn([2, 3, 5, 7, 11])
let invalidColumn = column / "foo"
print(invalidColumn.isValid) // Prints "false"
```

Important

A mismatch between the underlying types of two columns, or between the underlying type of a column and the type of a value, will result in an invalid column.

Once a column becomes invalid, you can’t use it for any subsequent operation because it will only produce further invalid columns or invalid tables.

Each comparison operator of MLUntypedColumn returns a column of Booleans. However, MLUntypedColumn uses integers as its underlying type for columns of Booleans, because MLDataValue does not have a case for Bool.

For example, create an untyped column of Booleans using the less-than comparison operator(&lt;(_:_:)).

```
let column = MLUntypedColumn([2, 3, 5, 7, 11])
let lessThan5 = column 

Then print the column to see that its underlying `ValueType` is `Int`, and each Boolean value of `true` or `false` is represented in the column by an integer value of `1` or `0`, respectively.

```
print(lessThan5)
/* Prints...
 ValueType: Int
 Values:        [1, 1, 0, 0, 0]
 */
```

Use these untyped columns of Booleans just as you would with a typed column of Booleans (\`\`MLDataColumn\`\`\`\`\>\`) to:

- Filter another untyped column with subscript(_:)

- Logically combine with another untyped column of Booleans with the &amp;&amp;(_:_:) and ||(_:_:) operators

- Mask rows of an MLDataTable with its subscript(_:)

## Topics

### Creating an untyped column

init&lt;T>(repeating: T, count: Int)

Creates a new column with a repeating value.

init(repeating: MLDataValue, count: Int)

Creates a new column with a repeating value.

init(Range&lt;Int>)

Creates a new column of integers from a given range.

init(ClosedRange&lt;Int>)

Creates a new column of integers from a given closed range.

init&lt;S>(S)

Creates a new column from a given sequence of elements that can be converted to machine learning data values.

init&lt;S>(S)

Creates a new column from a given sequence of machine learning data values.

init()

Creates an empty, invalid column used to remove an existing column from a data table.

### Creating an untyped column by converting another column

init(ints: MLUntypedColumn)

Creates a new column of integers by converting the elements of another column.

init(doubles: MLUntypedColumn)

Creates a new column of doubles by converting the elements of another column.

init(strings: MLUntypedColumn)

Creates a new column of strings by converting the elements of another column.

init(sequences: MLUntypedColumn)

Creates a new column of machine learning sequences by converting the elements of another column.

init(dictionaries: MLUntypedColumn)

Creates a new column of machine learning dictionaries by converting the elements of another column.

init(multiArrays: MLUntypedColumn)

Creates a MLUntypedColumn of type MLMultiArray from the specified MLUntypedColumn if the values of the given MLUntypedColumn are convertible to MLDataValue.MultiArrayType.

### Getting the number of elements

var count: Int

The number of elements in the column.

var isEmpty: Bool

### Getting an element

subscript(Int) -> MLDataValue

Accesses the element at the given position.

### Appending to an untyped column

func append(contentsOf: MLUntypedColumn)

Appends the elements of the given column to the end of this column.

### Duplicating a column

func copy() -> MLUntypedColumn

Returns a new MLUntypedColumn by copying the original MLUntypedColumn

### Sorting elements to generate a column

func sort(byIncreasingOrder: Bool) -> MLUntypedColumn

Returns a new MLUntypedColumn containing values sorted by the specified order.

### Converting a column to generate a data column

func map&lt;T>(to: T.Type) -> MLDataColumn&lt;T>

Creates a new column of typed values by converting this untyped column to the given type.

### Exposing the underlying type to generate a data column

var type: MLDataValue.ValueType

The underlying type of the column.

var ints: MLDataColumn&lt;Int>?

A cloned data column of integers.

var doubles: MLDataColumn&lt;Double>?

A cloned data column of doubles.

var strings: MLDataColumn&lt;String>?

A cloned data column of strings.

var sequences: MLDataColumn&lt;MLDataValue.SequenceType>?

A cloned data column of machine learning sequences.

var dictionaries: MLDataColumn&lt;MLDataValue.DictionaryType>?

A cloned data column of machine learning dictionaries.

var multiArrays: MLDataColumn&lt;MLDataValue.MultiArrayType>?

A cloned data column of machine learning multi-arrays.

func column&lt;T>(type: T.Type) -> MLDataColumn&lt;T>?

Clones the column to a data column of the given type.

### Transforming elements to generate a data column

func map&lt;T>((MLDataValue) -> T) -> MLDataColumn&lt;T>

Creates a new column of typed values by applying the given thread-safe transform to every non-missing element of this untyped column.

func map&lt;T>((MLDataValue) -> T?) -> MLDataColumn&lt;T>

Creates a new column of typed values, potentially with missing values, by applying the given thread-safe transform to every non-missing element of this untyped column.

func mapMissing&lt;T>((MLDataValue) -> T?) -> MLDataColumn&lt;T>

Creates a new column of typed values by applying the given thread-safe transform to every element of this untyped column, including missing elements.

### Masking elements to generate an untyped column

subscript(MLDataColumn&lt;Bool>) -> MLUntypedColumn

Creates a subset of the column by masking its elements with a data column of Booleans.

subscript(MLUntypedColumn) -> MLUntypedColumn

Creates a subset of the column by masking its elements with another untyped column.

### Discarding elements to generate an untyped column

func dropMissing() -> MLUntypedColumn

Creates a subset of the column by removing all elements without a value.

func dropDuplicates() -> MLUntypedColumn

Creates a subset of the column by removing all duplicate elements.

### Selecting elements to generate an untyped column

subscript(Range&lt;Int>) -> MLUntypedColumn

Creates a subset of the column, given a range of elements.

subscript&lt;R>(R) -> MLUntypedColumn

Creates a subset of the column, given a range expression of elements.

func prefix(Int) -> MLUntypedColumn

Creates a subset of the column, given a number of initial elements.

func suffix(Int) -> MLUntypedColumn

Creates a subset of the column, given a number of final elements.

### Filling in missing elements to generate an untyped column

func fillMissing(with: MLDataValue) -> MLUntypedColumn

Creates a modified copy of the column such that every missing element is replaced with the given value.

### Evaluating elements to generate an untyped column

func materialize() throws -> MLUntypedColumn

Creates a new column by immediately evaluating any lazily applied data processing operations stored in the column.

### Combining columns to generate an untyped column

static func + (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column by adding each element in the first column to the corresponding element in the second column.

static func - (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column by subtracting each element in the second column from the corresponding element in the first column.

static func * (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column by multiplying each element in the first column by the corresponding element in the second column.

static func / (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column by dividing each element in the first column by the corresponding element in the second column.

### Combining a column with a value to generate an untyped column

static func + (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column by adding each element of the given column to the given value.

static func - (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column by subtracting the given value from each element of the given column.

static func * (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column by multiplying each element of the given column by the given value.

static func / (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column by dividing each element of the given column by the given value.

### Combining a value with a column to generate an untyped column

static func + (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column by adding the given value to each element of the given column.

static func - (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column by subtracting each element of the given column from the given value.

static func * (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column by multiplying the given value by each element of the given column.

static func / (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column by dividing the given value by each element of the given column.

### Comparing columns to generate an untyped column of booleans

static func == (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is equal to the corresponding element in the second column.

static func != (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is not equal to the corresponding element in the second column.

static func > (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is greater than the corresponding element in the second column.

static func &lt; (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is less than the corresponding element in the second column.

static func &lt;= (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is less than or equal to the corresponding element in the second column.

static func >= (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the first column is greater than or equal to the corresponding element in the second column.

### Comparing a column with a value to generate an untyped column of booleans

static func == (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is equal to the given value.

static func != (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is not equal to the given value.

static func > (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is greater than the given value.

static func &lt; (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is less than the given value.

static func &lt;= (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is less than or equal to the given value.

static func >= (MLUntypedColumn, any MLDataValueConvertible) -> MLUntypedColumn

Creates a column of Booleans by testing whether each element in the given column is greater than or equal to the given value.

### Comparing a value with a column to generate an untyped column of booleans

static func == (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is equal to each element in the given column.

static func != (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is not equal to each element in the given column.

static func > (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is greater than each element in the given column.

static func &lt; (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is less than each element in the given column.

static func &lt;= (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is less than or equal to each element in the given column.

static func >= (any MLDataValueConvertible, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by testing whether the given value is greater than or equal to each element in the given column.

### Combining columns of booleans to generate an untyped column of booleans

static func &amp;&amp; (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by performing a logical AND operation on each row of two columns of Booleans.

static func || (MLUntypedColumn, MLUntypedColumn) -> MLUntypedColumn

Creates a column of Booleans by performing a logical OR operation on each row of two columns of Booleans.

### Visualizing a column

func show() -> any MLStreamingVisualizable

Provides a visualization for the data in the column.

Deprecated

### Getting a description of an untyped column

var description: String

A text representation of the column.

var playgroundDescription: Any

A description of the column shown in a playground.

var debugDescription: String

A text representation of the column for debugging.

var customMirror: Mirror

A view of the column for Xcode Playgrounds and lldb.

### Handling untyped column errors

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

struct MLDataColumn

A column of typed values in a data table.

struct MLDataTable

A table of data for training or evaluating a machine learning model.

### Adding columns

func addColumn&lt;Element>(MLDataColumn&lt;Element>, named: String)

Adds a data column to the table.

struct MLDataColumn

A column of typed values in a data table.

func addColumn(MLUntypedColumn, named: String)

Adds an untyped column to the table.

