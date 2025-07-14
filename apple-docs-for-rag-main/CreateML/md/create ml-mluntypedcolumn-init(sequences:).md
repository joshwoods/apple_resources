

- Create ML
- MLUntypedColumn
-  init(sequences:) 

Initializer

# init(sequences:)

Creates a new column of machine learning sequences by converting the elements of another column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(sequences: MLUntypedColumn)
```

## Parameters 

`sequences`  

A column with elements that are convertible to Create ML sequences.

## Return Value

A new untyped column of doubles; otherwise an invalid column if any element of the given column cannot be converted to MLDataValue.SequenceType.

## Discussion

Use this initializer to create a column of sequences from another column. As an example, to create a column with this initializer, first start with a column that is convertible to sequences.

```
let intSequenceString = "[1, 2, 3]"
let intSequenceString2 = "[4, 5, 6]"
let stringsColumn = MLUntypedColumn([intSequenceString, intSequenceString2])

print(stringsColumn)
/* Prints...
 ValueType: String
 Values:        [[1, 2, 3], [4, 5, 6]]
 */
```

Then use init(sequences:) to convert the column to a column of sequences.

```
let sequenceColumn = MLUntypedColumn(sequences: stringsColumn)
print(sequenceColumn)
/* Prints...
 ValueType: Sequence
 Values:        [[DataValue(1), DataValue(2), DataValue(3)],
                 [DataValue(4), DataValue(5), DataValue(6)]]
 */
```

## See Also

### Creating an untyped column by converting another column

init(ints: MLUntypedColumn)

Creates a new column of integers by converting the elements of another column.

init(doubles: MLUntypedColumn)

Creates a new column of doubles by converting the elements of another column.

init(strings: MLUntypedColumn)

Creates a new column of strings by converting the elements of another column.

init(dictionaries: MLUntypedColumn)

Creates a new column of machine learning dictionaries by converting the elements of another column.

init(multiArrays: MLUntypedColumn)

Creates a MLUntypedColumn of type MLMultiArray from the specified MLUntypedColumn if the values of the given MLUntypedColumn are convertible to MLDataValue.MultiArrayType.

