

- Create ML
- MLDataColumn
-  init(column:) 

Initializer

# init(column:)

Creates a new column of doubles from a given column whose elements can be converted to doubles.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(column: MLDataColumn) where T : MLDataValueConvertible
```

Available when `Element` is `Double`.

## Parameters 

`column`  

An MLDataColumn of elements convertible to Double.

## Discussion

Use this initializer to create a column of doubles from another column. Start by creating a column that is convertible to a column of doubles.

```
let stringsColumn = MLDataColumn(["1.0", "2.0", "3.0", "4.0", "5.0"])
print(stringsColumn) // Prints ["1.0", "2.0", "3.0", "4.0", "5.0"]
```

Then use init(column:) to convert the column to a column of doubles.

```
let doublesColumn = MLDataColumn(column: stringsColumn)
print(doublesColumn) // Prints [1.0, 2.0, 3.0, 4.0, 5.0]
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

Creates a new column of arrays of doubles from a given column whose elements can be converted to an array of doubles.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of strings from a given column whose elements can be converted to strings.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of arrays of strings from a given column whose elements can be converted to an array of strings.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of machine learning sequences from a given column whose elements can be converted to sequences.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of machine learning dictionaries from a given column whose elements can be converted to dictionaries.

