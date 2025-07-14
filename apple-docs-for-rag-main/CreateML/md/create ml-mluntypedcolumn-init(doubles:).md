

- Create ML
- MLUntypedColumn
-  init(doubles:) 

Initializer

# init(doubles:)

Creates a new column of doubles by converting the elements of another column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(doubles: MLUntypedColumn)
```

## Parameters 

`doubles`  

A column with elements that are convertible to doubles.

## Return Value

A new untyped column of doubles; otherwise an invalid column if any element of the given column cannot be converted to Double.

## Discussion

Use this initializer to create a column of doubles from another column. As an example, to create a column with this initializer, first start with a column that is convertible to doubles.

```
let stringColumn = MLUntypedColumn(["1.0", "2.0", "3.0", "4.0", "5.0"])
print(stringColumn)
/* Prints...
 ValueType: String
 Values:        [1.0, 2.0, 3.0, 4.0, 5.0]
 */
```

Then use init(doubles:) to convert the column to a column of doubles.

```
let doublesColumn = MLUntypedColumn(doubles: stringColumn)
print(doublesColumn)
/* Prints...
 ValueType: Double
 Values:        [1.0, 2.0, 3.0, 4.0, 5.0]
 */
```

## See Also

### Creating an untyped column by converting another column

init(ints: MLUntypedColumn)

Creates a new column of integers by converting the elements of another column.

init(strings: MLUntypedColumn)

Creates a new column of strings by converting the elements of another column.

init(sequences: MLUntypedColumn)

Creates a new column of machine learning sequences by converting the elements of another column.

init(dictionaries: MLUntypedColumn)

Creates a new column of machine learning dictionaries by converting the elements of another column.

init(multiArrays: MLUntypedColumn)

Creates a MLUntypedColumn of type MLMultiArray from the specified MLUntypedColumn if the values of the given MLUntypedColumn are convertible to MLDataValue.MultiArrayType.

