

- Create ML
- MLDataColumn
-  init(repeating:count:) 

Initializer

# init(repeating:count:)

Constructs a new Column containing the specified number of a single, repeated MLDataValue.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(
    repeating repeatedValue: MLDataValue,
    count: Int
)
```

## See Also

### Creating a data column

init(repeating: Element, count: Int)

Creates a new column with a repeating element.

init&lt;S>(S)

Creates a new column from a given sequence of elements.

init()

Constructs an invalid Column.

