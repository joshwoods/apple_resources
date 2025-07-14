

- Create ML
- MLDataColumn
-  init(repeating:count:) 

Initializer

# init(repeating:count:)

Creates a new column with a repeating element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(
    repeating repeatedValue: Element,
    count: Int
)
```

## Parameters 

`repeatedValue`  

An initial value for every element in the new column.

`count`  

A number of elements to create for the new column.

## Discussion

Use this initializer to create a column of repeating elements with any type that conforms to MLDataValueConvertible, including integers, doubles, strings, arrays, and dictionaries.

```
let three5s = MLDataColumn(repeating: 5, count: 3)
print(three5s) // Prints [5, 5, 5]
```

## See Also

### Creating a data column

init(repeating: MLDataValue, count: Int)

Constructs a new Column containing the specified number of a single, repeated MLDataValue.

init&lt;S>(S)

Creates a new column from a given sequence of elements.

init()

Constructs an invalid Column.

