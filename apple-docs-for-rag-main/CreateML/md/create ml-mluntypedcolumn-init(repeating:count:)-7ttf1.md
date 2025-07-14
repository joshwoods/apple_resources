

- Create ML
- MLUntypedColumn
-  init(repeating:count:) 

Initializer

# init(repeating:count:)

Creates a new column with a repeating value.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(
    repeating repeatedValue: T,
    count: Int
) where T : MLDataValueConvertible
```

## Parameters 

`repeatedValue`  

An initial value for every element in the new column.

`count`  

The number of elements in the new column.

## Discussion

Use this initializer to create a column of repeating elements with any type that conforms to MLDataValueConvertible, including integers, doubles, strings, arrays, and dictionaries.

```
let three5s = MLUntypedColumn(repeating: 5, count: 3)
print(three5s)
/* Prints...
 ValueType: Int
 Values:        [5, 5, 5]
 */
```

## See Also

### Creating an untyped column

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

