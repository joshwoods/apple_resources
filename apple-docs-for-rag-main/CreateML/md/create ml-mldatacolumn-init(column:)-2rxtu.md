

- Create ML
- MLDataColumn
-  init(column:) 

Initializer

# init(column:)

Creates a new column of arrays of integers from a given column whose elements can be converted to an array of integers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(column: MLDataColumn) where T : MLDataValueConvertible
```

Available when `Element` is `[Int]`.

## Parameters 

`column`  

An MLDataColumn of elements convertible to an Array of Int.

## Discussion

Use this initializer to create a column of arrays of integers from another column. Start by creating a column that is convertible to a column of arrays of integers.

Then use init(column:) to convert the column to a column of arrays of integers.

```
let intsColumn = MLDataColumn(column: stringsColumn)
print(intsColumn) // Prints [1, 2, 3, 4, 5]
```

## See Also

### Creating a data column by converting another column

func map&lt;T>(to: T.Type) -> MLDataColumn&lt;T>

Creates a new column by converting this column to the given type.

init&lt;T>(column: MLDataColumn&lt;T>)

Creates a new column of integers from a given column whose elements can be converted to integers.

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

