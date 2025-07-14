

- Create ML
- MLUntypedColumn
-  init(\_:) 

Initializer

# init(\_:)

Creates a new column from a given sequence of machine learning data values.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(_ source: S) where S : Sequence, S.Element == MLDataValue
```

## Parameters 

`source`  

A sequence of data value daelements for the new column.

## Discussion

Use this initializer to create a column from a sequence of data values.

```
let dataValueOf2 = MLDataValue.int(2)
let dataValueOf3 = MLDataValue.int(3)
let dataValueOf5 = MLDataValue.int(5)
let dataValueOf7 = MLDataValue.int(7)
let dataValueOf11 = MLDataValue.int(11)

let sequence = [dataValueOf2,
                dataValueOf3,
                dataValueOf5,
                dataValueOf7,
                dataValueOf11
]

let sequenceColumn = MLUntypedColumn(sequence)
print(sequenceColumn)
/*
Prints...
 ValueType: Int
 Values:        [2, 3, 5, 7, 11]
 */
```

## See Also

### Creating an untyped column

init&lt;T>(repeating: T, count: Int)

Creates a new column with a repeating value.

init(repeating: MLDataValue, count: Int)

Creates a new column with a repeating value.

init(Range&lt;Int>)

Creates a new column of integers from a given range.

init(ClosedRange&lt;Int>)

Creates a new column of integers from a given closed range.

init&lt;S>(S)

Creates a new column from a given sequence of elements that can be converted to machine learning data values.

init()

Creates an empty, invalid column used to remove an existing column from a data table.

