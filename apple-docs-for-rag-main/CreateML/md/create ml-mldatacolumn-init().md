

- Create ML
- MLDataColumn
-  init() 

Initializer

# init()

Constructs an invalid Column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init()
```

## Discussion

Assigning an invalid Column to a column name in a DataTable will remove any Column previously stored under that name.

## See Also

### Creating a data column

init(repeating: Element, count: Int)

Creates a new column with a repeating element.

init(repeating: MLDataValue, count: Int)

Constructs a new Column containing the specified number of a single, repeated MLDataValue.

init&lt;S>(S)

Creates a new column from a given sequence of elements.

