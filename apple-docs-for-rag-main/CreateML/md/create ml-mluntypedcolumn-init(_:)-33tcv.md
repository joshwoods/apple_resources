

- Create ML
- MLUntypedColumn
-  init(\_:) 

Initializer

# init(\_:)

Creates a new column of integers from a given range.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(_ range: Range)
```

## Parameters 

`range`  

A range of integer elements for the new column.

## Discussion

Use this initializer to create a column of incrementing values from a range.

```
let rangeColumn = MLUntypedColumn(3..

## See Also

### Creating an untyped column

init&lt;T>(repeating: T, count: Int)

Creates a new column with a repeating value.

init(repeating: MLDataValue, count: Int)

Creates a new column with a repeating value.

init(ClosedRange&lt;Int>)

Creates a new column of integers from a given closed range.

init&lt;S>(S)

Creates a new column from a given sequence of elements that can be converted to machine learning data values.

init&lt;S>(S)

Creates a new column from a given sequence of machine learning data values.

init()

Creates an empty, invalid column used to remove an existing column from a data table.

