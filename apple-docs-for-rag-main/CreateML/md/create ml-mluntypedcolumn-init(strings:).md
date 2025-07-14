

- Create ML
- MLUntypedColumn
-  init(strings:) 

Initializer

# init(strings:)

Creates a new column of strings by converting the elements of another column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(strings: MLUntypedColumn)
```

## Parameters 

`strings`  

A column with elements that are convertible to string.

## Return Value

A new untyped column of doubles; otherwise an invalid column if any element of the given column cannot be converted to String.

## Discussion

Use this initializer to create a column of strings from another column. As an example, to create a column with this initializer, first start with a column that is convertible to strings.

```
let doublesColumn = MLUntypedColumn([1.0, 2.718, 3.14, 4.2, 5.1])
print(doublesColumn)
/* Prints...
 ValueType: Double
 Values:        [1.0, 2.718, 3.14, 4.2, 5.1]
 */
```

Then use init(strings:) to convert the column to a column of strings.

```
let stringsColumn = MLUntypedColumn(strings: doublesColumn)
print(stringsColumn)
/* Prints...
 ValueType: String
 Values:        [1, 2.718, 3.14, 4.2, 5.1]
 */
```

## See Also

### Creating an untyped column by converting another column

init(ints: MLUntypedColumn)

Creates a new column of integers by converting the elements of another column.

init(doubles: MLUntypedColumn)

Creates a new column of doubles by converting the elements of another column.

init(sequences: MLUntypedColumn)

Creates a new column of machine learning sequences by converting the elements of another column.

init(dictionaries: MLUntypedColumn)

Creates a new column of machine learning dictionaries by converting the elements of another column.

init(multiArrays: MLUntypedColumn)

Creates a MLUntypedColumn of type MLMultiArray from the specified MLUntypedColumn if the values of the given MLUntypedColumn are convertible to MLDataValue.MultiArrayType.

