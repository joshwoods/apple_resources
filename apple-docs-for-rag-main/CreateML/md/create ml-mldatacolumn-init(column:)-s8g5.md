

- Create ML
- MLDataColumn
-  init(column:) 

Initializer

# init(column:)

Creates a new column of machine learning dictionaries from a given column whose elements can be converted to dictionaries.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(column: MLDataColumn) where T : MLDataValueConvertible
```

Available when `Element` is `MLDataValue.DictionaryType`.

## Parameters 

`column`  

An MLDataColumn of elements convertible to MLDataValue.DictionaryType.

## Discussion

Use this initializer to create a column of dictionaries from another column. Start by creating a column that is convertible to a column of dictionaries.

```
let intDictionaryString = "{1:\"one\", 2:\"two\", 3:\"three\"}"
let intDictionaryString2 = "{4:\"four\", 5:\"five\", 6:\"six\"}"
let stringsColumn = MLDataColumn([intDictionaryString, intDictionaryString2])

print(stringsColumn) // Prints ["{1:"one", 2:"two", 3:"three"}", "{4:"four", 5:"five", 6:"six"}"]
```

Then use init(column:) to convert the column to a column of dictionaries.

```
let dictionaryColumn = MLDataColumn(column: stringsColumn)
print(dictionaryColumn) // Prints [[1: one, 2: two, 3: three], [5: five, 4: four, 6: six]]
```

## See Also

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

