

- Create ML
- MLDataColumn
-  init(\_:) 

Initializer

# init(\_:)

Creates a new column from a given sequence of elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(_ source: S) where Element == S.Element, S : Sequence
```

## Parameters 

`source`  

A sequence of elements for the new column.

## Discussion

Use this initializer to create a column from a sequence of any type that conforms to MLDataValueConvertible.

```
let sequenceColumn = MLDataColumn([2, 3, 5, 7, 11])
print(sequenceColumn) // Prints [2, 3, 5, 7, 11]
```

## See Also

### Creating a data column

init(repeating: Element, count: Int)

Creates a new column with a repeating element.

init(repeating: MLDataValue, count: Int)

Constructs a new Column containing the specified number of a single, repeated MLDataValue.

init()

Constructs an invalid Column.

