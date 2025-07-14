

- Create ML
- MLUntypedColumn
-  init(dictionaries:) 

Initializer

# init(dictionaries:)

Creates a new column of machine learning dictionaries by converting the elements of another column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(dictionaries: MLUntypedColumn)
```

## Parameters 

`dictionaries`  

A column with elements that are convertible to Create ML dictionaries.

## Return Value

A new untyped column of doubles; otherwise an invalid column if any element of the given column cannot be converted to MLDataValue.DictionaryType.

## Discussion

Use this initializer to create a column of dictionaries from another column. As an example, to create a column with this initializer, first start with a column that is convertible to dictionaries.

```
let intDictionaryString = "{1:\"one\", 2:\"two\", 3:\"three\"}"
let intDictionaryString2 = "{4:\"four\", 5:\"five\", 6:\"six\"}"
let stringsColumn = MLUntypedColumn([intDictionaryString, intDictionaryString2])

print(stringsColumn)
/* Prints...
 ValueType: String
Values: [{1:"one", 2:"two", 3:"three"}, {4:"four", 5:"five", 6:"six"}]
 */
```

Then use init(dictionaries:) to convert the column to a column of dictionaries.

```
let dictionaryColumn = MLUntypedColumn(dictionaries: stringsColumn)
print(dictionaryColumn)
/* Prints...
 ValueType: Dictionary
 Values:        [[1: one, 3: three, 2: two], [4: four, 5: five, 6: six]]
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

init(sequences: MLUntypedColumn)

Creates a new column of machine learning sequences by converting the elements of another column.

init(multiArrays: MLUntypedColumn)

Creates a MLUntypedColumn of type MLMultiArray from the specified MLUntypedColumn if the values of the given MLUntypedColumn are convertible to MLDataValue.MultiArrayType.

