

- Create ML
- MLDataColumn
-  map(to:) 

Instance Method

# map(to:)

Creates a new column by converting this column to the given type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func map(to type: T.Type) -> MLDataColumn where T : MLDataValueConvertible
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`type`  

A type of MLDataColumn to convert the contents of the column to, using MLDataValueConvertible.

## Return Value

A new column.

## Discussion

This method is functionally equivalent to the initializers of MLDataColumn that have one parameter `column`, such as init(column:).

## See Also

### Creating a data column by converting another column

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

